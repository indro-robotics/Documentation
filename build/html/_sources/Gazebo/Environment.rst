.. toctree::
   :hidden:
   :titlesonly:


Creating an Environment
=============================

Creating a simple environment in Gazebo is very easy with the librarie's and tools inside the Gazebo simulation. Open up a new Gazebo session and start adding in shapes to the environment

1. The top bar navigation contains a square, sphere and cilindar shapes that can be added to the newly created world. The top bar also includes tools to adjust the shapes size, position and orientation. 

.. image:: navigationTop.png
	:width: 700
	:alt: Directory Layout
	:align: center


2. On the left navigation bar under the 'Insert' tab, there is a library of objects you can add to the world.

.. image:: stuff.png
	:width: 300
	:alt: Directory Layout
	:align: center


3. Here is an example of adding in objects and shapes to an empty world.

.. raw:: html

	<center>
		<video controls src="../_static/worldCreation.mp4" width="600"> </video>
	</center>
	
4. Delete models by selecting them and hitting the 'Delete' key

5. Save a world with 'Save World As' and choose sdf file option

6. Load a world with the command line

.. code-block:: text

	gazebo my_world.sdf

















