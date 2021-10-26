.. toctree::
   :hidden:



Ubuntu Installation
=======================

ROS Noetic requirs an Ubuntu 20.04. An easy way to do this is to create a virtual machine

*1. DOWNLOAD*

    * `VirtualBox <https://www.virtualbox.org/wiki/Downloads>`_ 
    * `Ubuntu Desktop <https://ubuntu.com/download/desktop>`_
    
    
*2. CREATE VM*

    In Virtual box, click the create new VM button, and make sure the bellow requirments are set before completing. 
    * 2GB-8GB of memory.
    * A new virtual hard disk
    * VDI
    * Dynamically allocated
    * 25GB-50GB

*3. MODIFY SETTINGS*

	* Navigate to settings/system/processor. Change the CPU amount from 1 CPU to 2-4

	* Navigate to settings/Network and change from NAT to Bridgeed Adapter to set up internet

*4. START*

    Start your VM, and when prompted, add the Ubuntu desktop downloaded previously.

