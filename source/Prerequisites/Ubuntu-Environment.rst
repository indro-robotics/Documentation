.. toctree::
   :hidden:



Ubuntu Installation
=======================

ROS Noetic requirs an Ubuntu 20.04. Ros Melodic requires ubuntu 18.04. An easy way to do this is to create a virtual machine. Download the Virtualbox app as well as one of the desktops 20.04 or 18.04 depending on which ROS version you want. We recomend Noetic for personal use as it is the most recent and up to date, while also giving users access to the most recent version of Gazebo. However ROS Melodic is required for our AgileX gazebo simulations.

*1. DOWNLOAD*

    * `VirtualBox <https://www.virtualbox.org/wiki/Downloads>`_ 
    * `Ubuntu Desktop 20.04 <https://ubuntu.com/download/desktop>`_
    * `Ubuntu Desktop 18.04 <https://releases.ubuntu.com/18.04/>`_
    
*2. CREATE VM*

In Virtual box, click the create new VM button, and make sure the bellow requirments are set before completing. 

    * 2GB-8GB of memory.
    * A new virtual hard disk
    * VDI
    * Dynamically allocated
    * 25GB-50GB
    
.. image:: vmcreat.gif
	:width: 500
	:alt: Directory Layout
    

*3. MODIFY SETTINGS*

	* Navigate to settings/system/processor. Change the CPU amount from 1 CPU to 2-4
	
	.. image:: procesors.gif
		:width: 500
		:alt: Directory Layout	


	* Navigate to settings/Network and change from NAT to Bridgeed Adapter to set up internet

	.. image:: adaptor.gif
		:width: 500
		:alt: Directory Layout	


	* Navigate to settings/Storage and add in the virtual disk downloaded previously

	.. image:: disk.gif
		:width: 500
		:alt: Directory Layout	

*4. START*

    Start your VM by double clicking on navigation bar, or by pressing start button. When prompted, procead to "Install Ubuntu" option and compleat configuration.


.. image:: install.gif
	:width: 500
	:alt: Directory Layout	




