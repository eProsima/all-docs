.. _docker_usage:

Docker Installation and Usage
-----------------------------

To run *eProsima DDS Suite* container, Docker is required.
From a terminal run

.. code-block:: bash

    sudo apt install docker.io

To load this image into your Docker repository, from a terminal run

.. code-block:: bash

    docker load -i ubuntu-eprosima-dds-suite:<version>.tar

*eProsima DDS Suite* Docker container can be run as follows:

.. code-block:: bash

    xhost local:root
    docker run \
        -it \
        --privileged \
        -e DISPLAY=$DISPLAY \
        -v /tmp/.X11-unix:/tmp/.X11-unix \
        ubuntu-eprosima-dds-suite:<version>

Each feature can be run from the resulting Bash Shell.

.. _eprosima_dds_suite_examples:

Fast DDS Examples
-----------------

Included in this Docker container is a set of binary examples that showcase several functionalities of the
*Fast DDS* library.
These examples' path can be accessed from a terminal by typing

.. code-block:: bash

    goToExamples

This will change the working directory to a location containing several examples, both for DDS and RTPS.
Below are the steps to launch two such examples.

Hello World Example
^^^^^^^^^^^^^^^^^^^

This is a minimal example that will perform a Publisher/Subscriber match and start sending samples.

.. code-block:: bash

    goToExamples
    cd HelloWorldExample/bin
    tmux new-session \
        "./HelloWorldExample publisher 0 1000" \; \
        split-window "./HelloWorldExample subscriber" \; \
        select-layout even-vertical

This example is not constrained to the current image instance, meaning that it is possible to run several instances of
this container to check the communication between them.
From one terminal you could launch an image and, on the presented shell, run:

.. code-block:: bash

    goToExamples
    cd HelloWorldExample/bin
    ./HelloWorldExample publisher

And then from another terminal with another instance run the following:

.. code-block:: bash

    goToExamples
    cd HelloWorldExample/bin
    ./HelloWorldExample subscriber

Benchmark Example
^^^^^^^^^^^^^^^^^

This example creates either a Publisher or a Subscriber and, after a successful match, starts sending samples.
After a few seconds the process that launched the Publisher will show a report with the number of samples transmitted.

On the subscriber side, run:

.. code-block:: bash

    goToExamples
    cd Benchmark/bin
    ./Benchmark subscriber udp

On the publisher side, run:

.. code-block:: bash

    goToExamples
    cd Benchmark/bin
    ./Benchmark publisher udp

.. _eprosima_dds_suite_shapes_demo:

Shapes Demo
-----------

To launch the *Shapes Demo*, from a terminal run:

.. code-block:: bash

    ShapesDemo

*eProsima Shapes Demo* usage information can be found on the `Shapes Demo documentation
<https://eprosima-shapes-demo.readthedocs.io/en/latest/first_steps/first_steps.html>`_.

.. _eprosima_dds_suite_monitor:

Fast DDS Monitor
----------------

To launch the *Fast DDS Monitor*, from a terminal run:

.. code-block:: bash

    fastdds_monitor

*eProsima Fast DDS Monitor* User Manual can be located on the `Fast DDS Monitor documentation
<https://fast-dds-monitor.readthedocs.io/en/latest/rst/user_manual/initialize_monitoring.html>`_.

.. _eprosima_dds_router:

DDS Router
----------

In this example the DDS Router is configured to communicate a publisher and subscriber running in different DDS Domains.

Run the following command to create the DDS Router *yaml* configuration file (``/config.yml``).

.. code-block:: bash

    echo "version: v2.0
    participants:
      - name: simple_dds_participant_0
        kind: local
        domain: 0
      - name: simple_dds_participant_1
        kind: local
        domain: 1" > /config.yml

Then execute the following command to run the Publisher in Domain 0, the Subscriber in Domain 1, and the
DDS Router communicating both Domains.

.. code-block:: bash

    goToExamples
    cd DDS/BasicConfigurationExample/bin
    tmux new-session \
        "ddsrouter --config-path /config.yml" \; \
        split-window -h "./BasicConfigurationExample publisher --domain 0 --interval 1000 --transport udp" \; \
        split-window -v "./BasicConfigurationExample subscriber --domain 1 --transport udp"

.. _micro_xrce_dds:

eProsima Micro XRCE-DDS
-----------------------

To launch the *Micro XRCE-DDS Agent*, from a terminal run:

.. code-block:: bash

    MicroXRCEAgent udp4 -p 2019 -r /root/agent.refs &

With the Agent started, you can now run the *Shapes Demo* application:

.. code-block:: bash

    ShapesDemo &

And launch the ShapeDemoClient, a demo client used to send data to *Shapes Demo* via the *Micro XRCE-DDS Agent*.

.. code-block:: bash

    ShapeDemoClient --udp4 127.0.0.1 2019

Inside that client, you can now follow the steps detailed in the `eProsima XRCE-DDS Shapes Demo page
<https://micro-xrce-dds.docs.eprosima.com/en/latest/shapes_demo.html>`_ to send data to *Shapes Demo*.

.. _plotjuggler_eprosima_edition:

PlotJuggler eProsima Edition
----------------------------

To launch the PlotJuggler eProsima Edition, from a terminal run:

.. code-block:: bash

 $ plotjuggler

eProsima PlotJuggler eProsima Edition usage information can be found on the `PlotJuggler eProsima Edition User Manual
<https://plotjuggler-fastdds-plugins.readthedocs.io/en/latest/>`_.
