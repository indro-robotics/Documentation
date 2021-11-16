.. toctree::
   :hidden:
   :titlesonly:


Gazebo Simulation
=============================

1. Enter limo_ws folder

.. code-block:: text

	cd limo_ws

2. Declare environment variables

.. code-block:: text

	source devel/setup.bash
	
3. Simulate

.. code-block:: text

	roslaunch limo_gazebo_sim limo_ackerman.launch


A simulation environment with the Limo robot should appear

.. image:: limo.png
	:width: 600
	:alt: Directory Layout


4. Drive Limo

Locate the rqt_robot_steering_RobotSteering window. If can't locate, open new tab in terminal and execute the following command.

.. code-block:: text

	rosrun rqt_robot_steering rqt_robot_steering

The Limo steering window should appear

.. image:: steering.png
	:width: 600
	:alt: Directory Layout

This window will allow you to control the movement of the robot using ackermann_steering_controller. The vertical bar acts as the forward, backwards movement needed to boost the robot into motion, while the horizontal bar controls the direction the robot accelerates in. Zoom in on the Hunter and play around with the controlls!



