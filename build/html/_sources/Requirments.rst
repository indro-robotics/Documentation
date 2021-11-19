.. _RequirmentsAgileX:

**Requirments**
=================

You need to have **Gazebo** and **ROS** downloaded before executing any of the commands. Visit our ROS and Gazebo pages for information on how to install.

Please execute the following code blocks in a new Terminal window to simulate these products


.. code-block:: text
	:caption: ros-control function package:

	sudo apt-get install ros-noetic-ros-control
	

.. code-block:: text
	:caption: ros-controllers function package:

	sudo apt-get install ros-noetic-ros-controllers


.. code-block:: text
	:caption: gazebo-ros function package:

	sudo apt-get install ros-noetic-gazebo-ros


.. code-block:: text
	:caption: gazebo-ros-control function package:

	sudo apt-get install ros-noetic-gazebo-ros-control..


.. code-block:: text
	:caption: rqt-robot-steering plug-in:

	sudo apt-get install ros-noetic-rqt-robot-steering 

.. code-block:: text
	:caption: keyboard controller:

	sudo apt-get install ros-melodic-teleop-twist-keyboard 


|

**AgileX Workspace**

In order to run the simulations, you will need the entire AgileX workspace. Open up a terminal. Navigate to the place you would like to store your AgileX simulation folder and execute the following commands in order. 


1. Create a new directory for your workspace

.. code-block:: text

	mkdir AgileX_ws

2. Enter AgileX_ws folder

.. code-block:: text

	cd AgileX_ws
	
3. Create a src folder

.. code-block:: text

	mkdir src
	
4. Enter src folder

.. code-block:: text

	cd src

5. Initialize catkin folder

.. code-block:: text

	catkin_init_workspace

6. Clone git simulation model package

.. code-block:: text

	git clone https://github.com/agilexrobotics/ugv_gazebo_sim.git


8. Enter AgileX_ws folder

.. code-block:: text

	cd ..	


9. Compile

.. code-block:: text

	catkin_make





















