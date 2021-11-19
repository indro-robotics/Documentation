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

	roslaunch ranger_mini_gazebo ranger_mini_empty_world.launch

A Gazebo simulation environment with the Ranger robot should appear

.. image:: ranger.png
	:width: 500
	:alt: Directory Layout
	:align: center

4. Drive Ranger

Use the Ackerman_steering_controller window to control the movement of the robot. The vertical bar acts as the forward, backwards movement needed to boost the robot into motion, while the horizontal bar controls the direction the robot accelerates in.

.. image:: steering.png
	:width: 500
	:alt: Directory Layout
	:align: center

|

Ranger Simulation
--------------------

.. raw:: html

	<center>
		<video controls src="../_static/ranger.mp4" width="600"> </video>
	</center>
	


	
