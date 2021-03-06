---
title: Installing PredictionIO
---

## Method 1: Launch an AWS Instance

You can [launch PredictionIO on Amazon Web Services](launch-aws.html).
This is a hassle-free way to get a well-configured PredictionIO server quickly.

## Method 2: Quick Install

On Linux / Mac OS X, PredictionIO can now be installed with a single command:
<br />
`$ bash -c "$(curl -s https://install.prediction.io/install.sh)"`

The above script will complete the rest of the instructions on this page for you
and you can proceed to the [Choosing an Engine
Template](/start/download).

## Method 3: Manual Install

### Prerequisites

It is **very important** to meet the minimum version of the following
technologies that power PredictionIO.

* Apache Hadoop 2.4.0 (optional, required only if YARN and HDFS are needed)
* Apache Spark 1.3.0 for Hadoop 2.4
* Java SE Development Kit 7

and one of the following sets:

* PostgreSQL 9.1

or

* MySQL 5.1

or

* Apache HBase 0.98.6
* Elasticsearch 1.4.0

If you are running on a single machine, we recommend a minimum of 2GB memory.

INFO: If you are using Linux, Apache Spark local mode, which is the default
operation mode without further configuration, may not work. In that case,
configure your Apache Spark to run in [standalone cluster
mode](http://spark.apache.org/docs/latest/spark-standalone.html).

### Installing PredictionIO

PredictionIO runs on a Java virtual machine, so it runs on most platforms.
Choose your platform below:

* [Installing PredictionIO on Linux / Mac OS X](install-linux.html)
* [Installing PredictionIO from Source Code](install-sourcecode.html)
* [Installing PredictionIO with Vagrant (VirtualBox)](install-vagrant.html)
* [Installing PredictionIO with Terminal.com Snap](https://www.terminal.com/snapshot/f444bfb7538dfc596485374f56167ec6f79cbc16f793f013ad120067070eb81a)


You may also use one of the community-contributed packages to install
PredictionIO:

* [Installing PredictionIO with
  Docker](/community/projects.html#docker-installation-for-predictionio)


[//]: # (* *(coming soon)* Installing PredictionIO with Homebrew)



WARNING: **0.8.2 contains schema changes from the previous versions, if you have
installed the previous versions, you may need to clear both HBase and
Elasticsearch. See more [here](/resources/upgrade/).**


[//]: # (## Production Deployment)

[//]: # (For production environment setup, please refer to [Production)
[//]: # (Deployment](/production/deploy.html) guide.)

## Method 4: Terminal.com

Public snaps are available on our Terminal.com
[page](https://www.terminal.com/user/predictionio).

Instance type **must be** set to *medium* or higher for PredictionIO to function
correctly.
