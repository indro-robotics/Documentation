.. toctree::
   :hidden:
   


ROS Node
=========================

**WHAT IS A NODE**

A node is a process that performs computation. For example, a node could control the motion plan, or the camera driver of a robot. There exists many different nodes inside one robot, each with a unique task and able to communicate with eachother.

**CREATE PYTHON NODE**

Create a new directory called scripts in your robot package, and this is where you will create your first python node in.

.. image:: firstNode.png
	:width: 700
	:alt: setup.bash

You can now open up your new python file in any text editor you want, and use python to write you're node functionalities. The following file is a template for a general node.

.. code-block::
	
	#!/usr/bin/env python
	import rospy
	if __name__=='__main__':
		rospy.init_node("pyton_node_name") #initializing the node. The name must be unique.
		rospy.loginfo("This node has been started")
		rospy.sleep(1)
		rate=rospy.Rate(10)
		while not rospy.is_shutdown():
			rospy.loginfo("Hello")
			rate.sleep()



The node is initialized with **rospy.init_node("name of node")**. The while loop keeps the node active.

Before executing your node, you must run the ros master in another terminal. Open up a new terminal and type 'roscore'. Then return to your terminal and run your python file with 'python my_first_node.py'. You can use 'roslist' command in another terminal to view active nodes.

.. image:: nodeTerminal.gif
	:width: 700
	:alt: setup.bash








