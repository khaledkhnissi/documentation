# How to setup the Computer

This guide helps you setup your computer for running the competition environment locally and developing the code.

You can use local Computer/Laptop or Virtual Machine inside your computer or any cloud platform like [Google GCP](https://cloud.google.com/free){target=_blank}, [Amazon AWS](https://aws.amazon.com/free/){target=_blank}, [Microsoft Azure](https://azure.microsoft.com/en-us/free/){target=_blank}, [Digital Ocean](https://try.digitalocean.com/freetrialoffer/){target=_blank}, etc (All Cloud providers have some free trial plan which you can make use of).
## System requirements

The competition setup needs to be run on [Ubuntu](https://ubuntu.com/download){target=_blank}, a flavor of [Linux](https://en.wikipedia.org/wiki/Linux){target=_blank}. You will need a computer that has:
    
- A dedicated [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit){target=_blank},
    - Nvidia cards tend to work well in Ubuntu
- A CPU that is at least an Intel i5, or equivalent,
- At least 4GB of free disk space,
- At least 8GB of RAM,
- Ubuntu Xenial installed.

## Operating System
If not already installed, Install **[Ubuntu Bionic (18.04)](https://releases.ubuntu.com/bionic/){target=_blank}** on the system by following [this guide](https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview){target=_blank}.

!!! note
    It is highly recommended to install [ Bionic (18.04)](https://releases.ubuntu.com/bionic/){target=_blank} version of Ubuntu due to [ROS (Melodic)](http://wiki.ros.org/melodic){target=_blank} dependency.

## Installing ROS
You need to install ROS Melodic by following [this guide](http://wiki.ros.org/melodic/Installation/Ubuntu){target=_blank} and install `ros-melodic-desktop-full` in the step `1.4` of the guide.

<!-- Abbrevations used in this page -->
*[ROS]: Robot Operating System
*[GCP]: Google Cloud Platform
*[AWS]: Amazon Web Services
*[GPU]: Graphics Processing Unit
*[CPU]: Central Processing Unit
