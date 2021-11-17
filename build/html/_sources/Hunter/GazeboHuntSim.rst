.. toctree::
   :hidden:
   :titlesonly:


Gazebo Simulation
=============================


1. Enter AgileX_ws folder

.. code-block:: text

	cd AgileX_ws

2. Declare environment variables

.. code-block:: text

	source devel/setup.bash
	
3. Simulate

.. code-block:: text

	roslaunch hunter2_gazebo hunter2_gazebo.launch
	

A simulation environment with the hunter robot should appear

.. image:: hunter.png
	:width: 600
	:alt: Directory Layout


4. Drive Hunter

Locate the rqt_robot_steering_RobotSteering window

.. image:: steering.png
	:width: 600
	:alt: Directory Layout

This window will allow you to control the movement of the robot using ackermann_steering_controller. The vertical bar acts as the forward, backwards movement needed to boost the robot into motion, while the horizontal bar controls the direction the robot accelerates in. Zoom in on the Hunter and play around with the controlls!


.. raw:: html

	<video controls src="_static/hunter.webm"></video>



	



