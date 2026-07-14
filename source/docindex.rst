.. role:: sr-only

.. raw:: html

    <div style="height: 40px;"></div>

.. image:: /01-figures/logo_eprosima_horizontal_1954x472.png
   :align: center
   :width: 95%
   :alt: eProsima - The middleware experts
   :class: only-light
   :target: `eProsima website`_

.. image:: /01-figures/logo_eprosima_horizontal_white_1954x472.png
   :align: center
   :width: 95%
   :alt: eProsima - The middleware experts
   :class: only-dark
   :target: `eProsima website`_

.. raw:: html

    <div style="height: 30px;"></div>

eProsima documentation index
----------------------------

eProsima is focused on developing middleware and tools for high performance distributed systems and its products are
customer driven.
Over the years, eProsima has excelled in several areas of expertise: low latency, high throughput, small footprint, low
bandwidth consumption, optimum protocol, low CPU use, etc., working under various scenarios, from high-performance
systems with high speed reliable links, to small devices connected over unreliable radio links.

Commercial support
------------------

.. |commercial_support_link| raw:: html

   <a href="https://forms.eprosima.com/reach/form/CommercialSupportRequest/formperma/Ac8GwewD7PTDadQZIV92qDEzNFfMlJnYmA029mSJtJ8" target="_blank" rel="noopener noreferrer">share your details</a>

Looking for commercial support? Please |commercial_support_link| so we can assist you.

.. |eprosima_webpage_link| raw:: html

   <a href="https://www.eprosima.com" target="_blank" rel="noopener noreferrer">eProsima’s webpage</a>

Find more about us at |eprosima_webpage_link|.

------------------------------------------------------------------------------------------------------------------------

.. rst-class:: docs-tile

|eProsima Fast DDS|_ :sr-only:`eProsima Fast DDS`
---------------------------------------------------

*eProsima Fast DDS* is a high performance publish subscribe open-source framework to share data in distributed systems
using a decoupled model based on Publishers, Subscribers, and Data Topics.

.. rst-class:: docs-tile

|eProsima Fast DDS Pro|_ :sr-only:`eProsima Fast DDS Pro`
-----------------------------------------------------------

*eProsima Fast DDS Pro* is the commercial edition of *eProsima Fast DDS*, created for industrial and defense
applications that require advanced networking capabilities.

.. rst-class:: docs-tile

|eProsima Safe DDS|_ :sr-only:`eProsima Safe DDS`
---------------------------------------------------

*eProsima Safe DDS* is a functionally safe, highly reliable, and efficient C++
implementation of the DDS protocol, designed for critical applications
in industries such as automotive, avionics, and medical devices,
ensuring compliance with the most stringent functional
safety standards like ISO 26262 ASIL D.

.. rst-class:: docs-tile

|eProsima Micro XRCE-DDS|_ :sr-only:`eProsima Micro XRCE-DDS`
---------------------------------------------------------------

*eProsima Micro XRCE-DDS* implements DDS-XRCE protocol specified in the
DDS for *eXtremely Resource Constrained Environments* proposal submitted
to the Object Management Group (OMG) consortium.

.. rst-class:: docs-tile

|eProsima Fast DDS Monitor|_ :sr-only:`eProsima Fast DDS Monitor`
-------------------------------------------------------------------

*eProsima Fast DDS Monitor* is a graphical desktop application aimed at monitoring DDS environments deployed using the
`eProsima Fast DDS`_ library.
Thus, the user can monitor in real time the status of publication/subscription communications between DDS entities.
They can also choose from a wide variety of communication parameters to be measured (latency, throughput, packet
loss, etc.), as well as record and compute in real time statistical measurements on these parameters (mean, variance,
standard deviation, etc.).

.. rst-class:: docs-tile

|eProsima Fast DDS Monitor Pro|_ :sr-only:`eProsima Fast DDS Monitor Pro`
---------------------------------------------------------------------------

*eProsima Fast DDS Monitor Pro* is the commercial edition of *eProsima Fast DDS Monitor*, designed for professional
deployments that require advanced monitoring capabilities and a richer user experience.

.. rst-class:: docs-tile

|eProsima DDS Router|_ :sr-only:`eProsima DDS Router`
-------------------------------------------------------

*eProsima DDS Router* is an application based on `eProsima Fast DDS`_ that allows
to connect DDS networks that belong to different LANs.
It works as a bridge between two or more DDS isolated configurations, and transfer
all the data from one to the other.
This capability could be used to create a bridge between an internal LAN and
external WAN communication, to allow DDS communication via internet.

.. rst-class:: docs-tile

|eProsima DDS Record & Replay|_ :sr-only:`eProsima DDS Record & Replay`
-------------------------------------------------------------------------

*eProsima DDS Record & Replay* is an end-user software application that efficiently saves DDS data published into a DDS environment in a MCAP format database.
Thus, the exact playback of the recorded network events is possible as the data is linked to the timestamp at which the original data was published.
This tool is easily configurable and installed with a default setup, so that DDS topics, data types and entities are automatically discovered without the need to specify the types of data recorded.

.. rst-class:: docs-tile

|eProsima Fast DDS Spy|_ :sr-only:`eProsima Fast DDS Spy`
-----------------------------------------------------------

*eProsima Fast DDS Spy* is a CLI interactive tool that allows to introspect a DDS network in human readable format.
It is possible to query the network about the DomainParticipants connected, their endpoints (DataWriters and DataReaders) and the topics they communicate in.
It is also possible to see the user data sent through network topics in a schematic format in run time.

.. rst-class:: docs-tile

|eProsima Shapes Demo|_ :sr-only:`eProsima Shapes Demo`
---------------------------------------------------------

*eProsima Shapes Demo* is an *eProsima Fast DDS* application that Publishes and Subscribes to shapes of
different colors and sizes moving on a board.
Each Shape conforms its own topic: Square, Triangle or Circle.
A single instance of the Shapes Demo can publish on or subscribe to several topics at a time.

.. rst-class:: docs-tile

|eProsima Fast CDR|_ :sr-only:`eProsima Fast CDR`
---------------------------------------------------

*eProsima FastCDR* is a C++ library that provides two serialization mechanisms.
One is the standard CDR serialization mechanism, while the other is a faster implementation that modifies the standard.

.. rst-class:: docs-tile

|eProsima DDS Suite|_ :sr-only:`eProsima DDS Suite`
-----------------------------------------------------

:ref:`eProsima DDS Suite <eprosima_dds_suite>` is a Docker image distributed by eProsima to provide a convenient
demonstration for several eProsima products.
This image includes: `eProsima Fast DDS`_, `eProsima Shapes Demo`_, `eProsima Fast DDS Monitor`_ and `eProsima DDS Router`_.

.. rst-class:: docs-tile

|eProsima Fast DDS Statistics Backend|_ :sr-only:`eProsima Fast DDS Statistics Backend`
-----------------------------------------------------------------------------------------

*eProsima Fast DDS Statistics Backend* is a C++ library to collect data from the
`eProsima Fast DDS`_ Statistics module, and generate statistical information
that applications can query.

.. rst-class:: docs-tile

|eProsima DDS Enabler|_ :sr-only:`eProsima DDS Enabler`
---------------------------------------------------------

*eProsima DDS Enabler* acts as a bridge between DDS networks and external systems,
it automatically discovers DDS topics/types, translates DDS data into a target data model,
and manages the underlying DDS participants, thus enabling real-time, 
two-way integration between DDS and other platforms.

.. rst-class:: docs-tile

`eProsima Discovery Server`_
----------------------------------------

*eProsima Discovery Server* is an `eProsima Fast DDS`_ discovery mechanism.
*eProsima Fast DDS* allows a centralized, non-standard, client-server discovery mechanism that:

.. rst-class:: indented-bullets

- extends *eProsima Fast DDS* use to non-unicast network transports like TCP, and

- speeds up the discovery-stage in a large number of participants scenarios.

.. rst-class:: docs-tile

`eProsima Integration Service`_
----------------------------------

*eProsima Integration Service* is a library based on `eProsima Fast DDS`_ for creating parameterized communication
bridges between different systems, services, and protocols.
It is also able to perform transformations over the messages such as customized routing and mapping.

.. rst-class:: docs-tile

`eProsima Non-Intrusive DDS Recorder`_
----------------------------------------

*eProsima Non-Intrusive DDS Recorder* is a tool to record all the DDS traffic in the network, using a non-intrusive
mechanism allowing the user to test, analyze or log the DDS distributed systems without adding any new DDS participant
or service, ensuring the recording of the real behavior and timing.

.. _eProsima website: https://www.eprosima.com/
.. _eProsima Fast DDS: https://fast-dds.docs.eprosima.com/
.. _eProsima Fast DDS Pro: https://fast-dds.docs.eprosima.com/en/latest/02-formalia/titlepage.html#fast-dds-pro
.. _eProsima Safe DDS: https://safe-dds.docs.eprosima.com/
.. _eProsima Micro XRCE-DDS: https://micro-xrce-dds.readthedocs.io/en/latest/
.. _eProsima Fast DDS Monitor: https://fast-dds-monitor.readthedocs.io/en/latest/
.. _eProsima Fast DDS Monitor Pro: https://fast-dds-monitor.readthedocs.io/en/latest/rst/formalia/titlepage.html#fast-dds-monitor-pro
.. _eProsima DDS Router: https://eprosima-dds-router.readthedocs.io/en/latest/
.. _eProsima DDS Record & Replay: https://dds-recorder.readthedocs.io/en/latest/
.. _eProsima Fast DDS Spy: https://fast-dds-spy.readthedocs.io/en/latest/
.. _eProsima Shapes Demo: https://eprosima-shapes-demo.readthedocs.io/
.. _eProsima Fast CDR: https://github.com/eProsima/Fast-CDR/releases/
.. _eProsima DDS Suite: dds-suite/intro.html
.. _eProsima Fast DDS Statistics Backend: https://fast-dds-statistics-backend.readthedocs.io/en/latest/
.. _eProsima DDS Enabler: https://dds-enabler.readthedocs.io/en/latest/
.. _eProsima Discovery Server: https://fast-dds.docs.eprosima.com/en/latest/fastdds/discovery/discovery_server.html
.. _eProsima Integration Service: https://integration-services.readthedocs.io/en/latest/
.. _eProsima Non-Intrusive DDS Recorder: https://www.eprosima.com/docs/non-intrusive-dds-recorder/1.0.0/pdf/User-Manual.pdf
.. _eProsima Fast DDS QoS Profiles Manager: https://fast-dds-qos-profiles-manager.readthedocs.io/en/latest/
.. _PlotJuggler eProsima Edition: https://plotjuggler-fastdds-plugins.readthedocs.io/en/latest/

.. |eProsima Fast DDS| image:: /02-tool-logos/fast-dds-logo-large.png
   :alt: eProsima Fast DDS
   :height: 45px

.. |eProsima Fast DDS Pro| image:: /02-tool-logos/fast-dds-pro-logo-large.png
   :alt: eProsima Fast DDS Pro
   :height: 45px

.. |eProsima Safe DDS| image:: /02-tool-logos/Safe-DDS-logo_transparent_trimmed.png
   :alt: eProsima Safe DDS
   :height: 45px

.. |eProsima Micro XRCE-DDS| image:: /02-tool-logos/Micro-XRCE-DDS-logo_transparent_trimmed.png
   :alt: eProsima Micro XRCE-DDS
   :height: 45px

.. |eProsima Fast DDS Monitor| image:: /02-tool-logos/fastdds-monitor-logo_trimmed.png
   :alt: eProsima Fast DDS Monitor
   :height: 60px

.. |eProsima Fast DDS Monitor Pro| image:: /02-tool-logos/fastdds-monitor-pro-logo_trimmed.png
   :alt: eProsima Fast DDS Monitor Pro
   :height: 60px

.. |eProsima DDS Router| image:: /02-tool-logos/DDS-Router-Logo_trimmed.png
   :alt: eProsima DDS Router
   :height: 45px

.. |eProsima DDS Record & Replay| image:: /02-tool-logos/DDS-Record-Replay-Logo_horizontal_trimmed.png
   :alt: eProsima DDS Record & Replay
   :height: 45px

.. |eProsima Fast DDS Spy| image:: /02-tool-logos/DDS-Spy-Logo_trimmed.png
   :alt: eProsima Fast DDS Spy
   :height: 48px

.. |eProsima Shapes Demo| image:: /02-tool-logos/ShapesDemo-Logo_horizontal_trimmed.png
   :alt: eProsima Shapes Demo
   :height: 45px

.. |eProsima Fast CDR| image:: /02-tool-logos/FastCDR-Logo_trimmed_transparent.png
   :alt: eProsima Fast CDR
   :height: 45px

.. |eProsima DDS Suite| image:: /02-tool-logos/DDS-Suite-Logo_horizontal_trimmed.png
   :alt: eProsima DDS Suite
   :height: 45px

.. |eProsima Fast DDS Statistics Backend| image:: /02-tool-logos/Fast-DDS-Statistics-Backend-Logo_horizontal_trimmed.png
   :alt: eProsima Fast DDS Statistics Backend
   :height: 50px

.. |eProsima DDS Enabler| image:: /02-tool-logos/DDS-Enabler-Logo_trimmed.png
   :alt: eProsima DDS Enabler
   :height: 48px

