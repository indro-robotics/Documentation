.. toctree::
   :hidden:
   :titlesonly:


Hunter Setup
==============

1. Create a new directory for your workspace

.. code-block:: text

	mkdir hunter_ws

2. Enter hunter_ws folder

.. code-block:: text

	cd hunter_ws
	
3. Create a src folder

.. code-block:: text

	mkdir src
	
4. Enter src folder

.. code-block:: text

	cd src

5. Initialize catkin folder

.. code-block:: text

	catkin_init_workspace

6. Clone git simulation model package

.. code-block:: text

	git clone https://github.com/agilexrobotics/ugv_gazebo_sim.git



8. Enter hunter_ws folder

.. code-block:: text

	cd ..


8.5 If you need common3-graphics

.. code-block:: text

	sudo apt-get update
	sudo apt-get install lsb-release
	sudo sh -c 'echo "deb http://packages.osrfoundation.org/gazebo/ubuntu-stable `lsb_release -cs` main" > /etc/apt/sources.list.d/gazebo-stable.list'
	wget http://packages.osrfoundation.org/gazebo.key -O - | sudo apt-key add -
	sudo apt-get update
	sudo apt-get install libignition-physics-dev
	sudo apt-get install libignition-common3-dev
	

9. Compile

.. code-block:: text

	catkin_make























