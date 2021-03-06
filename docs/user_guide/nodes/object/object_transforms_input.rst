Object Transforms Input
=======================

Description
-----------
This node returns the current location, rotation, and scale of the input object.

.. image:: images/object_transforms_input_node.png
   :width: 160pt

Inputs
------

- **Object** - An object.

Outputs
-------
- **Location** - A vector that contains the current location of the input object.
- **Rotation** - An euler that contains the current rotation of the input object.
- **Scale** - A vector that contains the current scale of the input object.
- **Quaternion** - A quaternion that contains the current rotation of the input object.

Advanced Node Settings
----------------------

- **Use Current Transformations** - If this option is disabled the the node will have an extra input **Frame** which define the frame at which the transformations is output.
- **Frame** - The value can either be **Absolute** or **Offset**, Absolute will return the transformations at the choosen frame. Offset will return the transformations at the choosen frame relative to the current frame.

Notes
-----

- To be able to use the quaternion output the rotation mode of the object have to be set to quaternion. The same for Euler's rotation.

Examples of Usage
-----------------

.. image:: gifs/object_transforms_input_node_example.gif
