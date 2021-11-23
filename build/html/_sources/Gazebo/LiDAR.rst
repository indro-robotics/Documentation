.. toctree::
   :hidden:
   :titlesonly:


Construct a LiDAR
=============================

Lidar is a method for determining ranges by targeting an object with a laser and measuring the time for the reflected light to return to the receiver. Useing math and algorithms, a robot can understand the distance of objects around it, and therefor learn how to navigate these objects in the real world. 


1. Open a terminal and create a folder for the LiDAR model

.. code-block:: text

	mkdir GazeboProj
	cd GazeboProj
	

2. Import code for model from GitHub

.. code-block:: text

	git init
	git clone https://github.com/EllaHayashiIndro/Lidar_Gazebo.git
	

3. Enter Lidar Folder

.. code-block:: text

	cd Lidar_Gazebo

4. Run the LiDAR world

.. code-block:: text

	gazebo lidar.world


5. View the Lidar working in Gazebo

.. raw:: html

	<center>
		<video controls src="../_static/lidar.mp4" width="600"> </video>
	</center>
	




This tutorial is based on a tutorial by `Gazebo <https://www.python.org/about/gettingstarted/>`_













































