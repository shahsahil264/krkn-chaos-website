---
title: Installation
description: 
categories: [Installation]
tags: [install, docs]
weight: 2
---

<!-- {{% pageinfo %}}
This is a placeholder page that shows you how to use this template site.
{{% /pageinfo %}} -->

The following ways are supported to run Kraken:
- Standalone python program through Git.
- Containerized version using either Podman or Docker as the runtime via [Krkn-hub](https://github.com/krkn-chaos/krkn-hub)
- Kubernetes or OpenShift deployment ( unsupported )

{{% alert title="Note" %}} It is recommended to run Kraken external to the cluster ( Standalone or Containerized ) hitting the Kubernetes/OpenShift API as running it internal to the cluster might be disruptive to itself and also might not report back the results if the chaos leads to cluster's API server instability.{{% /alert %}}

{{% alert title="Note" %}} To run Kraken on Power (ppc64le) architecture, build and run a containerized version by following the instructions given [here](https://github.com/krkn-chaos/krkn/blob/main/containers/build_own_image-README.md).{{% /alert %}}

{{% alert title="Note" %}} Helper functions for interactions in Krkn are part of [krkn-lib](https://github.com/krkn-chaos/krkn-lib). Please feel free to reuse and expand them as you see fit when adding a new scenario or expanding the capabilities of the current supported scenarios. {{% /alert %}}


## Prerequisites

Are there any system requirements for using your project? What languages are supported (if any)? Do users need to already have any software or tools installed?

## Installation

#### Git 
###### Clone the repository
```bash
$ git clone https://github.com/krkn-chaos/krkn.git --branch <release version>
$ cd krkn 
```
###### Install the dependencies

```bash
$ python3.9 -m venv chaos
$ source chaos/bin/activate
$ pip3.9 install -r requirements.txt
```
{{% alert title="Note" %}} Make sure python3-devel and latest pip versions are installed on the system. The dependencies install has been tested with pip >= 21.1.3 versions.{{% /alert %}}
Where can your user find your project code? How can they install it (binaries, installable package, build from source)? Are there multiple options/versions they can install and how should they choose the right one for them?

## Running Krkn

```bash
$ python3.9 run_kraken.py --config <config_file_location>
```

## Run containerized version

[Krkn-hub](https://github.com/krkn-chaos/krkn-hub) is a wrapper that allows running Krkn chaos scenarios via podman or docker runtime with scenario parameters/configuration defined as environment variables.



