:orphan:

.. _eprosima_suite:

eProsima Suite
==============

eProsima provides the eProsima Suite Docker image for those who want a Docker image with a set of eProsima's tools
and libraries running on an Ubuntu platform. It can be downloaded from
`eProsima's downloads page <https://eprosima.com/index.php/downloads-all>`_.

This Docker image was built for Ubuntu 20.04 (Focal Fossa).

To run this container you need Docker installed. From a terminal run

.. code-block:: bash

    $ sudo apt install docker.io

This Docker image contains the complete eProsima Suite. This includes:

- :ref:`eProsima Fast DDS libraries and examples <fast_dds_suite_examples>`: Fast DDS libraries bundled with several
  examples that showcase a variety of capabilities of eProsima's Fast DDS implementation.

- :ref:`Shapes Demo <fast_dds_suite_shapes_demo>`: eProsima Shapes Demo is an application in which Publishers and
  Subscribers are shapes of different colors and sizes moving on a board. Each shape refers to its own topic: Square,
  Triangle or Circle. A single instance of the eProsima Shapes Demo can publish on or subscribe to several topics at
  a time.

  You can read more about this application on the `Shapes Demo documentation page
  <https://eprosima-shapes-demo.readthedocs.io/>`_.

- :ref:`Fast DDS Monitor <fast_dds_suite_monitor>`: eProsima Fast DDS Monitor is a graphical desktop application aimed
  at monitoring DDS environments deployed using the *eProsima Fast DDS* library. Thus, the user can monitor in real
  time the status of publication/subscription communications between DDS entities. They can also choose from a wide
  variety of communication parameters to be measured (latency, throughput, packet loss, etc.), as well as record and
  compute in real time statistical measurements on these parameters (mean, variance, standard deviation, etc.).

  You can read more about this application on the `Fast DDS Monitor documentation page
  <https://fast-dds-monitor.readthedocs.io/>`_.

- :ref:`eProsima Micro XRCE-DDS <micro_xrce_dds>`:
  eProsima Micro XRCE-DDS is a software solution that allows communicating
  eXtremely Resource Constrained Environments (XRCEs) with an existing DDS network. This implementation complies with
  the specification of the `eXtremely Resource Constrained Environments DDS (DDS-XRCE)
  <https://www.omg.org/spec/DDS-XRCE/>`_. protocol as defined and maintained by the Object Management Group (OMG)
  consortium.

  You can read more about this application on the
  `eProsima Micro XRCE-DDS documentation page <https://micro-xrce-dds.docs.eprosima.com/>`_.

To load this image into your Docker repository, from a terminal run

.. code-block:: bash

 $ docker load -i ubuntu-eprosima-suite:<FastDDS-Version>.tar

You can run this Docker container as follows

.. code-block:: bash

 $ xhost local:root
 $ docker run -it --privileged -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix \
 ubuntu-eprosima-suite:<FastDDS-Version>

From the resulting Bash Shell you can run each feature.

.. _fast_dds_suite_examples:

Fast DDS Examples
-----------------

Included in this Docker container is a set of binary examples that showcase several functionalities of the
Fast DDS libraries. These examples' path can be accessed from a terminal by typing

.. code-block:: bash

 $ goToExamples

From this folder you can access all examples, both for DDS and RTPS. We detail the steps to launch two such
examples below.

Hello World Example
^^^^^^^^^^^^^^^^^^^

This is a minimal example that will perform a Publisher/Subscriber match and start sending samples.

.. code-block:: bash

 $ goToExamples
 $ cd HelloWorldExample/bin
 $ tmux new-session "./HelloWorldExample publisher 0 1000" \; \
 split-window "./HelloWorldExample subscriber" \; \
 select-layout even-vertical

This example is not constrained to the current instance. It's possible to run several instances of this
container to check the communication between them by running the following from each container.

.. code-block:: bash

 $ goToExamples
 $ cd HelloWorldExample/bin
 $ ./HelloWorldExample publisher

or

.. code-block:: bash

 $ goToExamples
 $ cd HelloWorldExample/bin
 $ ./HelloWorldExample subscriber

Benchmark Example
^^^^^^^^^^^^^^^^^

This example creates either a Publisher or a Subscriber and on a successful match starts sending samples. After a
few seconds the process that launched the Publisher will show a report with the number of samples transmitted.

On the subscriber side, run:

.. code-block:: bash

 $ goToExamples
 $ cd Benchmark/bin
 $ ./Benchmark subscriber udp

On the publisher side, run:

.. code-block:: bash

 $ goToExamples
 $ cd Benchmark/bin
 $ ./Benchmark publisher udp

.. _fast_dds_suite_shapes_demo:

Shapes Demo
-----------

To launch the Shapes Demo, from a terminal run

.. code-block:: bash

 $ ShapesDemo

eProsima Shapes Demo usage information can be found on the `Shapes Demo documentation
<https://eprosima-shapes-demo.readthedocs.io/en/latest/first_steps/first_steps.html>`_.

.. _fast_dds_suite_monitor:

Fast DDS Monitor
----------------

To launch the Fast DDS Monitor, from a terminal run

.. code-block:: bash

 $ fastdds_monitor

eProsima Fast DDS Monitor User Manual can be located on the `Fast DDS Monitor documentation
<https://fast-dds-monitor.readthedocs.io/en/latest/rst/user_manual/initialize_monitoring.html>`_.


.. _micro_xrce_dds:

eProsima Micro XRCE-DDS
-----------------------

To launch the Micro XRCE-DDS Agent, from a terminal run

.. code-block:: bash

 $ MicroXRCEAgent udp4 -p 2019 &

With the Agent started, you can now run the ShapesDemo

.. code-block:: bash

 $ ShapesDemo &

And launch the ShapeDemoClient, a demo client used to send data to the ShapesDemo via the Micro XRCE-DDS Agent.

.. code-block:: bash

 $ ShapeDemoClient --udp4 127.0.0.1 2019

Inside that client, you can now follow the steps detailed in the `eProsima XRCE-DDS Shapes Demo page
<https://micro-xrce-dds.docs.eprosima.com/en/latest/shapes_demo.html>`_ to send data to the ShapesDemo.



