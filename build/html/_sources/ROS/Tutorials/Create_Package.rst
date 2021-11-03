.. toctree::
   :hidden:



ROS Package
=========================


**WHAT IS A PACKAGE**

Packages will allow you to separate your code into reusable blocks. A package is an independant unit. For example, for one Robot, you can have multiple different packages, each handling a different application for the robot. One application might be handling the Robot camera, while the other might be handling the motion of the Robot.


**CREATE A ROS PACKAGE**

1. Enter src folder inside catkin workspace

.. code-block:: text

	cd src

2. Create a new package (e.g. package name is new_Package)

.. code-block:: text

	catkin_create_pkg new_Package roscpp rospy std_msgs


3. Navigate out of src folder

.. code-block:: text

	cd ..
	
3. You must always catkin_make after creating a new package

.. code-block:: text

	catkin_make


*Terminal output of creating a new package*

.. image:: create_catkin.png
	:width: 700
	:alt: Alternative test





