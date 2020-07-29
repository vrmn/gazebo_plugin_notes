NOTE: so far to my understanding plugins are C++ and directories are made in the home directory.

steps

1)create basic Model
this is done by ceating a .world file

this template is good to get things started.

<?xml version="1.0" ?>
<sdf version="1.5">
  <world name="default">

    <!-- A global light source -->
    <include>
      <uri>model://sun</uri>
    </include>

    <!-- A ground plane -->
    <include>
      <uri>model://ground_plane</uri>
    </include>
  </world>
</sdf>

you can then add the basic shapes for the sensor. refer to the velodyne world file and pay attention the <model>  tag
which has in it <link> <collision> <visual> <geometry>  <cylinder> <collsion> tags

Then fix the inertia

Then add the sensor

2) step two improve appearance with meshes

3) adding sensor noise

4) create the plugin for the sensor.
