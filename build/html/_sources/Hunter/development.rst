.. toctree::
   :hidden:
   :titlesonly:


Hunter Development
=============================

Convert Step file to URDF
----------------------------

1. download step file

2. If you don't already have FreeCad, download FreeCad to convert our step file


.. code-block:: text

	sudo apt-get install freecad
	sudo apt install python3-pyqt5

3. Open Hunter step file in FreeCad

.. code-block:: text

	freecad ~/Downloads/HDL32E_Outline_Model.STEP


.. image:: freecadHunter.png
	:width: 500
	:alt: Directory Layout
	:align: center

4. Select your model in the left tab under Applications, then export to STL

.. image:: stlHunter.png
	:width: 500
	:alt: Directory Layout
	:align: center



5. Make your model SDF file
































































