.. toctree::
   :hidden:
   :titlesonly:


Control plugin
=============================

We are going to create a plugin for the Velodyne LiDAR created in the previouse page. the plugin is a C++ library that is loaded by Gazebo at runtime. Plugin's are useful for developers because they let developers control almost any aspect of Gazebo, are self-contained routines, and can be inserted and removed from any system. A plugin created here can be re-used on a different model. You should always use a plugin when you want to alter a simulation.


Prerequisites
--------------------------

We will be using the model created in 'Construct a LiDAR' page to control this LiDAR plugin. We will also be using C++. Full understanding of C++ is not needed to follow the tutorial, but basic knowledge might be useful.



Install plugin packages
----------------------------------


.. code-block:: text

	sudo apt install libgazebo8-dev


.. code-block:: text

	sudo yum install gazebo-devel








