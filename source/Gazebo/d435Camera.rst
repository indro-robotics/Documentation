.. toctree::
   :hidden:
   :titlesonly:


RealSense d435 Camera Plugin
=================================

RealSense D435 camera is a camera with a wide field of view, along with a global shutter on the depth sensor that is ideal for fast moving applications.

.. image:: d435.png
	:width: 400
	:alt: Directory Layout
	:align: center

For more information on the Intel RealSense and their depth Camera D435 visit their site at the `Intel Website <https://www.intelrealsense.com/depth-camera-d435/>`_ 



Requirments
---------------------------

The user of this code will need an Ubuntu environment with ROS Noetic, and Gazebo installed. Additionally the user will need to install the following packages.


.. code-block:: text

	sudo apt install ros-noetic-xacro

.. code-block:: text

	sudo apt-get install ros-noetic-robot-state-publisher

.. code-block:: text

	sudo apt install ros-noetic-rviz


.. code-block:: text

	sudo apt-get install ros-noetic-cv-bridge

.. code-block:: text

	sudo apt-get install ros-noetic-control-toolbox



Gazebo Simulation
--------------------------------------

1. Create a new directory for the d435 code

.. code-block:: text

	mkdir realsense

2. Enter directory

.. code-block:: text

	cd realsense

3. Import code from Github

.. code-block:: text

	git init
	git clone https://github.com/EllaHayashiIndro/realsense_d435Camera.git

4. Make catkin link

.. code-block:: text

	catkin_make

5. Launch Gazebo Simulation

.. code-block:: text

	roslaunch realsense2_description view_d435_model_rviz_gazebo.launch

6. Navigate Simulation

.. raw:: html

	<center>
		<video controls src="../_static/d435.mp4" width="600"> </video>
	</center>









