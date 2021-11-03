.. toctree::
   :hidden:



Core Concepts
==============

On this page we will be discussing the high levle view of ROS, and not the technical details. It is essential to understand how the components work together to create the product you want. 

ROS works with independent nodes acting on their own and communicating with eachother. Nodes can handle any specific task that a robot might need, from motion control components to camera handling. There are also different types of node factions, such as publisher, subscriber, client, and server, which are specifically designed to act a certain way with other nodes. 

We also have a ROS Master, the most important component of the system. The ROS master is what allows the nodes to communicate with eachother. Upon starting the ROS master, the active nodes must register first with the master. The master will then direct which nodes to talk to which other nodes. This is why when starting the system, ROS developers must always have a ROS master active and running. 

Below is a conceptual example of what nodes connected to a ROS master might look like.

.. image:: ROS_Diagram.png
	:width: 700
	:alt: Directory Layout

In the diagram, the circular cells are all nodes connected and registered to the ROS master. They communicate to eachother in variouse ways, by either sending data directly to a node, or by subscribing and publishing to topics. The simple example diagram is a layout of a robot that moves with a motion plan based on an image that a camera gathers. 





