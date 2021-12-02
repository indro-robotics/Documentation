.. toctree::
   :hidden:
   :titlesonly:


ROS in Gazebo
=============================

ROS can be used in Gazebo to give your robot instructions and control

System Requirments
-----------------------------

You should have ROS and Gazebo preinstalled, as well as understand the basic concepts of ROS



Install gazebo_ros_pkgs
--------------------------------

gazebo_ros_pkgs will be able to let the developer run gazebo through rosrun command.

.. code-block:: text

	sudo apt-get install ros-noetic-gazebo-ros-pkgs ros-noetic-gazebo-ros-control


Test the install by running a roscore window, and then running a rosrun command in another window

.. code-block:: text

	roscore
	rosrun gazebo_ros gazebo

In a seperate tab you should be able to run rostopic list, and see the running gazebo state


.. image:: gazebo_ros_topic.png
	:width: 500
	:alt: Directory Layout
	:align: center



Launch a World With Roslaunch
-------------------------------------


























