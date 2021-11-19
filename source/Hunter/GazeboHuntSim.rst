.. toctree::
   :hidden:
   :titlesonly:


Launch Gazebo
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
	:width: 400
	:alt: Directory Layout
	:align: center


4. Drive Hunter

Use the Ackerman_steering_controller window to control the movement of the robot. The vertical bar acts as the forward, backwards movement needed to boost the robot into motion, while the horizontal bar controls the direction the robot accelerates in.

.. image:: steering.png
	:width: 400
	:alt: Directory Layout
	:align: center


|

Hunter Simulation
--------------------

.. raw:: html

	<center>
		<video controls src="../_static/hunter.mp4" width="600"> </video>
	</center>
	


	



