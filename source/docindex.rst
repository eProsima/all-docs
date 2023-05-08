.. image::  /01-figures/enhanced_logo.png
    :align: center
    :alt: eProsima - The middleware experts
    :target: `eProsima website`_

.. raw:: html

    <br><br><br><br>
    <h1>
        eProsima documentation index
    </h1>

eProsima is focused on developing middleware and tools for high performance distributed systems and its products are
customer driven.
Over the years, eProsima has excelled in several areas of expertise: low latency, high throughput, small footprint, low
bandwidth consumption, optimum protocol, low CPU use, etc., working under various scenarios, from high-performance
systems with high speed reliable links, to small devices connected over unreliable radio links.

------------------------------------------------------------------------------------------------------------------------

`eProsima Fast DDS`_
----------------------

*eProsima Fast DDS* is a high performance publish subscribe framework to share data in distributed systems using a
decoupled model based on Publishers, Subscribers, and Data Topics.

------------------------------------------------------------------------------------------------------------------------

`eProsima Safe DDS`_
----------------------

eProsima Safe DDS is a functionally safe, highly reliable, and efficient C++
implementation of the DDS protocol, designed for critical applications
in industries such as automotive, avionics, and medical devices,
ensuring compliance with the most stringent functional
safety standards like ISO 26262 ASIL D.

------------------------------------------------------------------------------------------------------------------------

`eProsima Micro XRCE-DDS`_
----------------------------

*eProsima Micro XRCE-DDS* implements DDS-XRCE protocol specified in the
DDS for *eXtremely Resource Constrained Environments* proposal submitted
to the Object Management Group (OMG) consortium.

------------------------------------------------------------------------------------------------------------------------

`eProsima Fast DDS Monitor`_
------------------------------

*eProsima Fast DDS Monitor* is a graphical desktop application aimed at monitoring DDS environments deployed using the
`eProsima Fast DDS`_ library.
Thus, the user can monitor in real time the status of publication/subscription communications between DDS entities.
They can also choose from a wide variety of communication parameters to be measured (latency, throughput, packet
loss, etc.), as well as record and compute in real time statistical measurements on these parameters (mean, variance,
standard deviation, etc.).

------------------------------------------------------------------------------------------------------------------------

`eProsima Fast DDS Statistics Backend`_
----------------------------------------

*eProsima Fast DDS Statistics Backend* is a C++ library to collect data from the
`eProsima Fast DDS`_ Statistics module, and generate statistical information
that applications can query.

------------------------------------------------------------------------------------------------------------------------

`eProsima DDS Router`_
----------------------------------

*eProsima DDS Router* is an application based on `eProsima Fast DDS`_ that allows
to connect DDS networks that belong to different LANs.
It works as a bridge between two or more DDS isolated configurations, and transfer
all the data from one to the other.
This capability could be used to create a bridge between an internal LAN and
external WAN communication, to allow DDS communication via internet.

------------------------------------------------------------------------------------------------------------------------

`eProsima Discovery Server`_
----------------------------------------

*eProsima Discovery Server* is an `eProsima Fast DDS`_ discovery mechanism.
*eProsima Fast DDS* allows a centralized, non-standard, client-server discovery mechanism that:

    - extends *eProsima Fast DDS* use to non-unicast network transports like TCP, and
    - speeds up the discovery-stage in a large number of participants scenarios.

------------------------------------------------------------------------------------------------------------------------

`eProsima Fast DDS QoS Profiles Manager`_
-------------------------------------------

*eProsima Fast DDS QoS Profiles Manager* is a tool suite for the generation of `eProsima Fast DDS`_ configuration files.
The suite provides both a Graphical User Interface (GUI) and a Command Line Interface (CLI).

------------------------------------------------------------------------------------------------------------------------

`eProsima Shapes Demo`_
---------------------------------

*eProsima Shapes Demo* is an *eProsima Fast DDS* application that Publishes and Subscribes to shapes of
different colors and sizes moving on a board.
Each Shape conforms its own topic: Square, Triangle or Circle.
A single instance of the Shapes Demo can publish on or subscribe to several topics at a time.

------------------------------------------------------------------------------------------------------------------------

`eProsima Fast CDR`_
----------------------------------

*eProsima FastCDR* is a C++ library that provides two serialization mechanisms.
One is the standard CDR serialization mechanism, while the other is a faster implementation that modifies the standard.

------------------------------------------------------------------------------------------------------------------------

`PlotJuggler eProsima Edition`_
----------------------------------------

*PlotJuggler eProsima Edition* is a plugin for PlotJuggler application to visualize DDS data by subscribing to selected
topics in a DDS network.
It uses Fast DDS Dynamic Types to introspect the data types and generate time series for every value in the topic.
It also supports several features to interact with data series and layouts.

------------------------------------------------------------------------------------------------------------------------

`eProsima DDS Suite`_
---------------------

:ref:`eProsima DDS Suite <eprosima_dds_suite>` is a Docker image distributed by eProsima to provide a convenient
demonstration for several eProsima products.
This image includes: `eProsima Fast DDS`_, `eProsima Shapes Demo`_, `eProsima Fast DDS Monitor`_,
`eProsima DDS Router`_, `eProsima Fast DDS QoS Profiles Manager`_ and `eProsima Micro XRCE-DDS`_.

------------------------------------------------------------------------------------------------------------------------

`eProsima Integration Service`_
----------------------------------

*eProsima Integration Service* is a library based on `eProsima Fast DDS`_ for creating parameterized communication
bridges between different systems, services, and protocols.
It is also able to perform transformations over the over the messages such as customized routing and mapping.

------------------------------------------------------------------------------------------------------------------------

`eProsima RPC over DDS`_
----------------------------------

*eProsima RPC over DDS* is a high performance Remote Procedure Call (RPC) framework.
It combines a software stack with a code generation engine to build services that work efficiently in several platforms
and programming languages.

------------------------------------------------------------------------------------------------------------------------

`eProsima Non-Intrusive DDS Recorder`_
----------------------------------------

*eProsima Non-Intrusive DDS Recorder* is a tool to record all the DDS traffic in the network, using a non-intrusive
mechanism allowing the user to test, analyze or log the DDS distributed systems without adding any new DDS participant
or service, ensuring the recording the real behavior and timing.

.. _eProsima website: https://www.eprosima.com/
.. _eProsima Fast DDS: https://fast-dds.docs.eprosima.com/en/latest/
.. _eProsima Safe DDS: https://safe-dds.docs.eprosima.com/
.. _eProsima Micro XRCE-DDS: https://micro-xrce-dds.readthedocs.io/en/latest/
.. _eProsima Fast DDS Monitor: https://fast-dds-monitor.readthedocs.io/en/latest/
.. _eProsima Fast DDS Statistics Backend: https://fast-dds-statistics-backend.readthedocs.io/en/latest/
.. _eProsima DDS Router: https://eprosima-dds-router.readthedocs.io/en/latest/
.. _eProsima Discovery Server: https://fast-dds.docs.eprosima.com/en/latest/fastdds/discovery/discovery_server.html
.. _eProsima Fast DDS QoS Profiles Manager: https://fast-dds-qos-profiles-manager.readthedocs.io/en/latest/
.. _eProsima Shapes Demo: https://eprosima-shapes-demo.readthedocs.io/en/latest/
.. _eProsima Fast CDR: https://www.eprosima.com/images/PDFs/Fast_CDR.pdf
.. _PlotJuggler eProsima Edition: https://plotjuggler-fastdds-plugins.readthedocs.io/en/latest/
.. _eProsima DDS Suite: dds-suite/intro.html
.. _eProsima Integration Service: https://integration-services.readthedocs.io/en/latest/
.. _eProsima RPC over DDS: https://www.eprosima.com/docs/rpc-over-dds/1.0.3/pdf/eprosima-fast-rtps/User-Manual.pdf
.. _eProsima Non-Intrusive DDS Recorder:    https://www.eprosima.com/docs/non-intrusive-dds-recorder/1.0.0/pdf/User-Manual.pdf
