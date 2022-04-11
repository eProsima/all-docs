:orphan:

.. _eprosima_dds_suite:

eProsima DDS Suite
==================

eProsima provides the *eProsima DDS Suite* Docker image for those who want a Docker image with a set of eProsima's tools
and libraries running on an Ubuntu platform.
It can be downloaded from `eProsima's downloads page <https://eprosima.com/index.php/downloads-all>`_.

This Docker image contains the complete *eProsima DDS Suite*, which includes:

- :ref:`eProsima Fast DDS library and examples <eprosima_dds_suite_examples>`: *Fast DDS* library bundled with several
  examples that showcase a variety of capabilities of eProsima's *Fast DDS* implementation.
  For more information about *Fast DDS* please refer to `Fast DDS documentation page
  <https://fast-dds.docs.eprosima.com/>`_

- :ref:`Shapes Demo <eprosima_dds_suite_shapes_demo>`: eProsima *Shapes Demo* is an application in which Publishers and
  Subscribers create and display shapes of different colors and sizes moving on a board.
  Each shape refers to its own topic: Square, Triangle or Circle.
  A single instance of the eProsima *Shapes Demo* can publish on and/or subscribe to several topics at a time.
  For more information about *Shapes Demo* please refer to `Shapes Demo documentation page
  <https://eprosima-shapes-demo.readthedocs.io/>`_.

- :ref:`Fast DDS Monitor <eprosima_dds_suite_monitor>`: eProsima *Fast DDS Monitor* is a graphical desktop application
  aimed at monitoring DDS environments deployed using the *eProsima Fast DDS* library.
  Thus, the user can monitor in real time the status of publication/subscription communications between DDS entities.
  They can also choose from a wide variety of communication parameters to be measured (latency, throughput,
  packet loss, etc.), as well as record and compute in real time statistical measurements on these parameters
  (mean, variance, standard deviation, etc.).
  For more information about *Fast DDS Monitor* please refer to `Fast DDS Monitor documentation page
  <https://fast-dds-monitor.readthedocs.io/>`_.

- :ref:`DDS Router <eprosima_dds_router>`: eProsima DDS Router is an end-user software application that enables the
  connection of distributed DDS networks.
  That is, DDS entities such as publishers and subscribers deployed in one geographic location and using a dedicated
  local network will be able to communicate with other DDS entities deployed in different geographic areas on their own
  dedicated local networks as if they were all on the same network through the use of eProsima DDS Router.
  This is achieved by deploying a DDS Router on an edge device of each local network so that the DDS Router routes DDS
  traffic from one network to the other through WAN communication.
  For more information about *DDS Router* please refer to
  `DDS Router documentation website <https://eprosima-dds-router.readthedocs.io>`_.

- :ref:`eProsima Micro XRCE-DDS <micro_xrce_dds>`:
  *eProsima Micro XRCE-DDS* is a software solution that allows communicating eXtremely Resource Constrained Environments
  (XRCEs) with an existing DDS network.
  This implementation complies with the specification of the `eXtremely Resource Constrained Environments DDS
  (DDS-XRCE) <https://www.omg.org/spec/DDS-XRCE/>`_ protocol as defined and maintained by the Object Management Group
  (OMG) consortium.
  For more information about *eProsima Micro XRCE-DDS* please refer to
  `eProsima Micro XRCE-DDS documentation page <https://micro-xrce-dds.docs.eprosima.com/>`_.

.. toctree::
    :caption: Getting started

    dds_suite
