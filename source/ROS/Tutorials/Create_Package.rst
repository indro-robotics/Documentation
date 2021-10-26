.. toctree::
   :hidden:



ROS Package
=========================


**WHAT IS A PACKAGE**

Packages will allow you to separate your code into reusable blocks. A package is an independant unit. For example, for one Robot, you can have multiple different packages, each handling a different application for the robot. One application might be handling the Robot camera, while the other might be handling the motion of the Robot.


**CREATE A ROS PACKAGE**

Navigate to the src folder of the catkin workspace, and to create a package, type catkin_create_pkg 'name_of_package' roscpp rospy std_msgs.

Always catkin_make after every created package!

.. image:: create_catkin.png
	:width: 700
	:alt: Alternative test





