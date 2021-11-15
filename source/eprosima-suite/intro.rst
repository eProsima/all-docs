:orphan:

.. _eprosima_suite:

eProsima Suite
==============

eProsima provides the eProsima Suite Docker image for those who want a Docker image with a set of eProsima's tools
and libraries running on an Ubuntu platform. It can be downloaded from
`eProsima's downloads page <https://eprosima.com/index.php/downloads-all>`_.

This Docker image contains the complete eProsima Suite. This includes:

- :ref:`eProsima Fast DDS libraries and examples <fast_dds_suite_examples>`: Fast DDS libraries bundled with several
  examples that showcase a variety of capabilities of eProsima's Fast DDS implementation.

- :ref:`Shapes Demo <fast_dds_suite_shapes_demo>`: eProsima Shapes Demo is an application in which Publishers and
  Subscribers create and display shapes of different colors and sizes moving on a board. Each shape refers to its own
  topic: Square, Triangle or Circle. A single instance of the eProsima Shapes Demo can publish on and/or subscribe to
  several topics at a time.

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
  <https://www.omg.org/spec/DDS-XRCE/>`_ protocol as defined and maintained by the Object Management Group (OMG)
  consortium.

  You can read more about this application on the
  `eProsima Micro XRCE-DDS documentation page <https://micro-xrce-dds.docs.eprosima.com/>`_.

.. toctree::
    :caption: Getting started

    eprosima_suite
