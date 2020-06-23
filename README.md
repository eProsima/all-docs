# eProsima projects documentation index

<a href="http://www.eprosima.com"><img src="https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcSd0PDlVz1U_7MgdTe0FRIWD0Jc9_YH-gGi0ZpLkr-qgCI6ZEoJZ5GBqQ" align="left" hspace="8" vspace="2" width="100" height="100" ></a>

*eprosima Fast DDS* (formerly Fast RTPS) is a C++ implementation of the DDS (Data Distribution Service) standard of the OMG (Object Management Group). eProsima Fast DDS implements the RTPS (Real Time Publish Subscribe) protocol, which provides publisher-subscriber communications over unreliable transports such as UDP,
as defined and maintained by the Object Management Group (OMG) consortium. RTPS is also the wire interoperability protocol defined for the Data Distribution
Service (DDS) standard. *eProsima Fast DDS* exposes an API to access the RTPS protocol directly, giving the user full access to the protocol internals.

Some of the main features of this library are:

* Configurable best-effort and reliable publish-subscribe communication policies for real-time
applications.
* Plug and play connectivity so that any new applications are automatically discovered by any other
members of the network.
* Modularity and scalability to allow continuous growth with complex and simple devices in the
network.
* Configurable network behavior and interchangeable transport layer: Choose the best protocol and
system input/output channel combination for each deployment.
* Two API Layers: a high-level Publisher-Subscriber one focused on usability (DDS) and a lower-level Writer-Reader one that provides finer access to the inner workings of the RTPS protocol.

*eProsima Fast DDS* has been adopted by multiple organizations in many sectors including these important cases:

* Robotics: ROS (Robotic Operating System) as their default middleware for ROS2.
* EU R&D: FIWARE Incubated GE.

You can find all the library's source code on our [GitHub repository](https://github.com/eProsima/Fast-DDS).

The documentation is built using [Sphinx](https://www.sphinx-doc.org), and it is hosted at [Read the Docs](https://readthedocs.org).
The online documentation generated with this project can be found in [eProsima projects documentation index](https://docs.eprosima.com/).

## Installation Guide

1. In order to build and test the documentation, some dependencies must be installed beforehand:

    ```bash
    sudo apt update
    sudo apt install -y \
        git \
        python3 \
        python3-pip \
        python3-venv \
        python3-sphinxcontrib.spelling \
    ```

1. Clone the repository

    ```bash
    cd ~
    git clone git@github.com:eProsima/all-docs.git all-docs
    ```

1. Create a virtual environment and install python3 dependencies

    ```bash
    cd ~/all-docs
    python3 -m venv all-docs-venv
    source all-docs-venv/bin/activate
    pip3 install -r docs/requirements.txt
    ```

## Getting Started

To generate the documentation in a HTML format for a specific branch of eProsima Shapes Demo run:

```bash
cd ~/all-docs
source all-docs-venv/bin/activate
make html
```

## Generating documentation in other formats

The documentation can be generated in several formats such as HTML, PDF, LaTex, etc. For a complete list of targets run:

```bash
cd ~/all-docs
make help
```

Once you have selected a format, generate the documentation with:

```bash
cd ~/all-docs
source all-docs-venv/bin/activate
make <output_format>
```

## Running documentation tests

This repository provides a set of tests that verify that:

1. The RST follows the style guidelines
1. There are no spelling errors
1. The HTML is built correctly

Run the tests by:

```bash
cd ~/all-docs
source all-docs-venv/bin/activate
make test
```
