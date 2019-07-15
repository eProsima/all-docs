.. all-docs documentation master file, created by
   sphinx-quickstart on Tue Dec 18 09:46:32 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

eProsima project documentation index
====================================

eProsima is focused in networking middleware and tools for high
performance distributed systems and our products are customer driven.
Over the years we have excelled in several areas of expertise: Low
latency, high throughput, small footprint, low bandwidth consumption,
optimum protocol, low cpu use, etc working under very different
scenarios, from high-performance systems with high speed reliable links,
to small devices connected over unreliable radio links.

.. image:: http://www.eprosima.com/images/boxes/Fast_RTPS_box200w.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Fast RTPS`_

----------------------
`eProsima Fast RTPS`_
----------------------

**eProsima Fast RTPS** is a high performance publish subscribe
framework to share data in distributed systems using a decoupled model
based on Publishers, Subscribers, and Data Topics.

.. image:: https://www.eprosima.com/images/screenshots/eProsima-Shapes-Demo.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Shape Demo`_

---------------------------------
`eProsima Shape Demo`_
---------------------------------

Shapes Demo is an application that Publishes and Subscribes to shapes of
different colors and sizes moving on a board. Each Shape conforms its
own topic: Square, Triangle or Circle. A single instance of the Shapes
Demo can publish on or subscribe to several topics at a time.

..  image:: logo.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Micro XRCE-DDS`_

----------------------------
`eProsima Micro XRCE-DDS`_
----------------------------

**eProsima Micro XRCE-DDS** implements **DDS-XRCE protocol** specified in the
DDS for *eXtremely Resource Constrained Environments* proposal submitted
to the **Object Management Group (OMG)** consortium.

..  image:: logo.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Integration Services`_

----------------------------------
`eProsima Integration Services`_
----------------------------------

**eProsima Integration Service** is a library based on `Fast RTPS`_ for
creating parameterized communication bridges between different systems,
services, and protocols. It is also able to perform transformations over
the over the messages such as customized routing and mapping.

..  image:: http://www.eprosima.com/images/boxes/RPC_over_DDS_box200.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima RPC over DDS`_

----------------------------------
`eProsima RPC over DDS`_
----------------------------------

**eProsima RPC over DDS is a high performance remote procedure call (RPC) framework**. It combines a software stack
with a code generation engine to build services that work efficiently in several platforms and programming languages.

..  image:: https://www.eprosima.com/images/boxes/Fast_Buffers_box200b.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Fast Buffers`_

----------------------------------
`eProsima Fast Buffers`_
----------------------------------

**eProsima Fast Buffers** is an **open source serialization engine optimized for performance**, beating alternatives
such as Apache Thrift and Google Protocol Buffers in both Simple and Complex Structures.

..  image:: logo.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Non-Intrusive DDS Recorder`_

----------------------------------------
`eProsima Non-Intrusive DDS Recorder`_
----------------------------------------

**eProsima Non-intrusive DDS Recorder** is a tool to record all the DDS traffic in your network, using a non-intrusive
mechanism allowing you to test, analyze or log your DDS distributed system without adding any new DDS participant or
service, ensuring you are recording the real behavior and timing.

..  image:: logo.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Dynamic Fast Buffers`_

----------------------------------------
`eProsima Dynamic Fast Buffers`_
----------------------------------------

**eProsima Dynamic Fast Buffers** is an **open source high-performance serialization library** using a different
approach to the traditional serialization frameworks. Data types are defined through a friendly API directly in your
application code, and the serialization support is generated at runtime.

..  image:: logo.png
    :height: 70
    :width: 70
    :align: left
    :target: `eProsima Discovery Server`_

----------------------------------------
`eProsima Discovery Server`_
----------------------------------------

**eProsima Discovery Server** is an application that simplifies the use and testing of the new `Fast RTPS`_
discovery capabilities.
Now Fast RTPS allows a centralized, non-standard, client-server discovery mechanism that:

- extends Fast RTPS use to non-unicast network transports like TCP.
- speeds up the discovery-stage in a large number of participants scenarios.


.. _eProsima Fast RTPS: http://eprosima-fast-rtps.readthedocs.io
.. _eProsima Shape Demo: https://eprosima-shapes-demo.readthedocs.io/en/latest/
.. _eProsima Micro XRCE-DDS: https://micro-xrce-dds.readthedocs.io/en/latest/introduction.html
.. _eProsima Integration Services: https://integration-services.readthedocs.io/en/latest/
.. _Fast RTPS: http://eprosima-fast-rtps.readthedocs.io
.. _eProsima RPC over DDS: https://www.eprosima.com/docs/rpc-over-dds/1.0.3/pdf/eprosima-fast-rtps/User-Manual.pdf
.. _eProsima Fast Buffers: https://www.eprosima.com/docs/fast-buffers/0.3.0/pdf/User-Manual.pdf
.. _eProsima Non-Intrusive DDS Recorder:    https://www.eprosima.com/docs/non-intrusive-dds-recorder/1.0.0/pdf/User-Manual.pdf
.. _eProsima Dynamic Fast Buffers: https://www.eprosima.com/docs/dynamic-fast-buffers/0.2.0/pdf/User-Manual.pdf
.. _eProsima Discovery Server: https://eprosima-discovery-server.readthedocs.io/en/latest/


