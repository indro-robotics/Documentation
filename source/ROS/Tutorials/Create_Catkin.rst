.. toctree::
   :hidden:


.. role:: underline
    :class: underline



Catkin Workspace
=========================

**WHAT IS A CATKIN WORKSPACE**

Catkin is the official build system for ROS. You will use it everytime you need to build your ROS application.


**CREATE CATKIN WORKSPACE**


To create a Catkin workspace please make sure you are in your home directory, or the directory that you choose to create your ROS program. 

1. Create a new catkin directory 

.. code-block:: text

	mkdir catkin_ws


2. Navigate inside catkin directory

.. code-block:: text

	cd catkin_ws
	
3. Make a src folder

.. code-block:: text

	mkdir src


4. Execute catkin_make command in src folder. This will build you a new ROS work environment. 

.. code-block:: text

	catkin_make


Now if you list all inside the catkin directory (using ls), you should see the created 'src' folder, a 'build' folder, and a 'devel' folder

.. image:: isCatkin.png
	:width: 700
	:alt: Directory Layout


5. Go into devel folder

.. code-block:: text

	cd devel


6. Set up bash

.. code-block:: text

	source setup.bash
	
	
That is all you need to create a new catkin workspace for ROS!







