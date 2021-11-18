.. toctree::
   :hidden:
   :titlesonly:


Installation
==============
This page explains how to install ROS on Ubuntu Linux.



System Requirments
-------------------

We will be using Ubuntu 20.04 / ROS Noetic / Python 3. For information on how to set up Ubuntu environment, and informatin on Linux Terminal/python 3, visit Prerequisites page.



Download ROS
----------------

Open up a new terminal and execute the following commands in order.


.. code-block:: text

	sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

.. code-block:: text

	sudo apt install curl
	
.. code-block:: text

	curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

.. code-block:: text

	sudo apt update

.. code-block:: text

	sudo apt install ros-noetic-desktop-full

.. code-block:: text

	echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc



Optional ROS Packages
-----------------------

These are recomended installs and required to follow the tutorial guides. 

.. code-block:: text

	sudo apt install ros-noetic-rosbash

.. code-block:: text

	sudo apt-get install ros-noetic-rqt-graph


You should have ROS downloaded on your device now! Navigate to the `ROS instalation page <http://wiki.ros.org/noetic/Installation/Ubuntu>`_ for any further information on the installation process.



Test ROS Download
---------------------

To test your newly installed ROS, start a ROS master by simply opening a new terminal and execute 'roscore'. You should see the following to know it is a success.

.. image:: roscore.png
	:width: 500
	:alt: Alternative test
	:align: center

To exit the roscore master, press Ctrl+C to kill the process.





















