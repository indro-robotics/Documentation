.. toctree::
   :hidden:



Ubuntu Installation
=======================

ROS Noetic requirs an Ubuntu 20.04. An easy way to do this is to create a virtual machine

To create an Ubuntu Virtual Machine, first download:
    * `VirtualBox <https://www.virtualbox.org/wiki/Downloads>`_ 
    * `Ubuntu Desktop <https://ubuntu.com/download/desktop>`_
    
Then create a new virtual machine in virtualbox with 
    * 2GB-8GB of memory.
    * A new virtual hard disk
    * VDI
    * Dynamically allocated
    * 25GB-50GB

In your new VM instance, navigate to settings/system/processor. Change the CPU amount from 1 CPU to 2-4

Then Navigate to settings/Network and change from NAT to Bridgeed Adapter to set up internet

Finally start your VM, and Add the disk image ubuntu desktop downloaded previously.

