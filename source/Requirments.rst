.. _RequirmentsAgileX:

**Requirments**
=================

**AgileX simulations require Ubuntu 18.04 + ROS Melodic desktop full**

There are a few required installations for use of the AgileX products in Gazebo. Please execute the following code blocks in a new Terminal window.

You also need to have **Gazebo** and **ROS** downloaded.

.. code-block:: text
	:caption: ros-control function package:

	sudo apt-get install ros-melodic-ros-control
	

.. code-block:: text
	:caption: ros-controllers function package:

	sudo apt-get install ros-melodic-ros-controllers


.. code-block:: text
	:caption: gazebo-ros function package:

	sudo apt-get install ros-melodic-gazebo-ros


.. code-block:: text
	:caption: gazebo-ros-control function package:

	sudo apt-get install ros-melodic-gazebo-ros-control


.. code-block:: text
	:caption: rqt-robot-steering plug-in:

	sudo apt-get install ros-melodic-rqt-robot-steering 


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





















