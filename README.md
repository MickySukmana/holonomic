# holonomic
holonomic robot simulation with ROS2 &amp; Gazebo  
  
This package currently use plannar move plugin to move the robot  

to run the package use:  
```
ros2 launch holonomic launch_sim.launch.py
```
The robot can be controlled by using keyboard with this command:
```
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```
  
  
  
to use high res model comment following line in robot.urdf.xacro:
```
<xacro:include filename="robot_core.xacro"/>
```
and uncomment this line:
```
<xacro:include filename="robot_core_highres.xacro"/>
```
