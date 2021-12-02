.. toctree::
   :hidden:
   :titlesonly:


Construct a LiDAR
=============================

Lidar is a method for determining ranges by targeting an object with a laser and measuring the time for the reflected light to return to the receiver. Useing math and algorithms, a robot can understand the distance of objects around it, and therefor learn how to navigate these objects in the real world. Our goal is to construct the model of the LiDAR, and then create a Plugin for the LiDAR

This tutorial is based on a tutorial by `Gazebo <https://www.python.org/about/gettingstarted/>`_


Create LiDAR Model
---------------------------------

1. Open a terminal and go to home directory

.. code-block:: text

	cd~
	

2. Import code for model from GitHub.

.. code-block:: text

	git init
	git clone  
	

3. Enter Lidar Folder

.. code-block:: text

	cd Lidar_Gazebo

4. View contents of folder. We can see all the imported files, including our LiDAR model which is named lidar.world. the lidar.world file contains all the information Gazebo needs to build the physical elements of the Lidar as well as the joints. The other files included in this folder will be for the plugin created in the next section

.. code-block:: text

	ls

.. image:: Terminal_Lidar.png
	:width: 600
	:alt: Directory Layout
	:align: center


5. Run the LiDAR world

.. code-block:: text

	gazebo lidar.world


6. View the Lidar working in Gazebo. We can manually alter the force in the tab on the right by changing the value's.

.. raw:: html

	<center>
		<video controls src="../_static/lidar.mp4" width="600"> </video>
	</center>
	
|

Create LiDAR Plugin
-------------------------------------------

We are going to create a plugin for the Velodyne LiDAR to control the sensor's one degree of freedom. This plugin is code for the LiDAR so that we do not have to manually change the force value on the right tab, and it will work on it's own. A plugin is a C++ library that is loaded by Gazebo at runtime. Plugin's are useful for developers because they let developers control almost any aspect of Gazebo, are self-contained routines, and can be inserted and removed from any system. A plugin created here can be re-used on a different model. You should always use a plugin when you want to alter a simulation programatically.



1. Install plugin packages for Gazebo 11

.. code-block:: text

	sudo apt install libgazebo11-dev


2. Enter the previously imported LiDAR workspace pulled from GitHub.

.. code-block:: text

	cd Lidar_Gazebo


3. View contents in the folder. We can see all our files.

.. code-block:: text

	ls

.. image:: Terminal_Lidar.png
	:width: 600
	:alt: Directory Layout
	:align: center


**velodyn_plugin.cc** 
	* This is our Lydar plugin file. The plugin contains information on how to control the Velodyne's joints for rotation. We want a configurable speed for the Lydar's rotation that doesn't require hardcoding in value's and re-compiling every time we want to change the speed. We also want to support  dynamic adjustment. To support dynamic adjustment we have an API built in the plugin. The API will allow our plugin to read messages passed from Gazebo's transport mechanism. In otherwords, a user in Gazebo adjusting the speed, will be able to send the value's to our plugin code, that will control the rotation spead of the LiDAR. The Lidar plugin code must therefor contain code that will accept changes in values. We also need a way for the users to send the value's dynamicall to the user. We have created a vel.cc script for this.
	
**vel.cc** 
	* This is our test API script that allows users to dynamically change the speed of the LiDAR's rotation. It does this by sending value's to the API created in velodyn_plugin.cc

**CMakeList.txt** 
	* This is a build script. A build script is a script that builds listed scripts in a planned order. Plugins need this script since they are independent code on their own. The file contains three builds and compiles them in order. It starts with 'Find Gazebo' where it connects to Gazebo, then proceads to 'Build our plugin' where it compiles our LiDAR Plugin code, and lastly it starts 'Build the stand-alone test program', where we can use this program to interface with our plugin.



4. Attach the plugin to the LiDAR model


.. code-block:: text
	:caption: open up model file

	gedit velodyne.world
	

.. code-block:: text
	:caption: add line of code right **before** </model> tag in script
	
	<plugin name="velodyne_control" filename="libvelodyne_plugin.so"/>


.. image:: pluginConf1.png
	:width: 600
	:alt: Directory Layout
	:align: center


Build and test plugin



.. code-block:: text
	:caption: Create build directory for make

	mkdir build


.. code-block:: text
	:caption: Compile plugin

	cmake ..
	make


"error" Could not find a package configuration file provided by "gazebo" with any of the following names:gazeboConfig.cmake gazebo-config.cmake

solution:

.. code-block:: text

	sudo apt install libgazebo11-dev









































