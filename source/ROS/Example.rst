.. toctree::
   :hidden:



Tutorial/Demonstration
========================

We will be demonstrating Turtlesim, an in ROS example, demonstrating the functionality of ROS

If its not already installed:

.. code-block:: text
	:caption: turtlesim:

	sudo apt-get install ros-noetic-turtlesim
	
You can play around with this example. First start rosmaster with roscore. Now you can launch nodes with rosrun. choose turtlesim_node. 	

if you also run turtle_teleop_key you can use key nodes.

you can see your nodes in rosnode list

rostopic list will also show you the topics

rqt_graph will show you the graph.

rosservice list will show you the lists of service nodes

ros service info /reset

rosservice call /reset ("TAB for info")

#rosservice list

#rosservice info /turtle1/teleport_relative

#rosservice call /turtle1/teleport_relative "linear:1.0 angular: 0.0"


go ahead and play and debut!!!
	















