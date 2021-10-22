.. toctree::
   :hidden:


Installation
==============
This page explains how to install ROS on Ubuntu Linux.


*System Requirments*
---------------------
We will be using Ubuntu 20.04 / ROS Noetic / Python 3. For information on how to set up Ubuntu environment, and informatin on Linux Terminal/python 3, visit Prerequisites page.


*Download ROS*
---------------------

Open up a new terminal and execute the following commands in order.


.. code-block:: text
	:caption: Step 1:

	sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

.. code-block:: text
	:caption: Step 2:

	sudo apt install curl
	
.. code-block:: text
	:caption: Step 3:

	curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

.. code-block:: text
	:caption: Step 4:

	sudo apt update

.. code-block:: text
	:caption: Step 5:

	sudo apt install ros-noetic-desktop-full

.. code-block:: text
	:caption: Step 6:

	echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc


You should have ROS downloaded on your device now! Navigate to the `ROS instalation page <http://wiki.ros.org/noetic/Installation/Ubuntu>`_ for any further information on the installation process.


*Test Download*
---------------------

To test your newly downloaded ROS, start a ROS master by simply opening a new terminal and execute 'roscore'. You should see the following to know it is a success.

.. image:: roscore.png
	:width: 700
	:alt: Alternative test

To exit the roscore master, press Ctrl+C to kill the process.





















