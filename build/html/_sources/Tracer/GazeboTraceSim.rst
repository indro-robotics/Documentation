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

	roslaunch tracer_gazebo_sim tracer_playpen.launch


A Gazebo simulation environment with the Tracer robot should appear

.. image:: tracer.png
	:width: 500
	:alt: Directory Layout
	:align: center

4. Open a new tab in terminal and run the keyboard controller

.. code-block:: text

	rosrun teleop_twist_keyboard teleop_twist_keyboard.py 

Use the terminal with the teleop_twist_keyboard controller to move the robot. The controls are listed as 'u', 'i','o', 'j', 'k', 'l', 'm', ',', and '.' on the keyboard.

.. image:: teleop.png
	:width: 500
	:alt: Directory Layout
	:align: center


5. Drive the Tracer

Have the terminal with the teleop_twist_keyboard.py infront of the Gazebo environment. The controller needs to be the active window. Use the Moving around keys to control the robot

.. image:: tracerSim.png
	:width: 500
	:alt: Directory Layout
	:align: center


Tracer Simulation
--------------------

.. raw:: html

	<center>
		<video controls src="../_static/Tracer.mp4" width="600"> </video>
	</center>
	





