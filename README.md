# Manipulator-Control
This repository contains packages for controlling the manipulators

# interbotix_xsrm_gazebo
This package is uesd to launch gazebo while other packages is used to conrtrol the manipulator in simulation.

# interbotix_xsarm_control
This package is used for control the manipulator through ros2.

To get started, open up a terminal and run the command below.
```console
ros2 launch interbotix_xsarm_control xsarm_control.launch.py robot_model:=px150
```
Then, in another terminal, navigate to the Python-ROS API demos directory and run the command.
```console
python3 bartender.py
```
You should observe the robot pick up a virtual bottle (from behind a virtual bar), rotate so that the end-effector is facing the opposite direction, pour a virtual drink (on the virtual bar), then place the ‘bottle’ down, and go to its Sleep pose.

If you want to test out your code first on a simulated arm, make sure to set the use_sim arg to true like this:
```console
ros2 launch interbotix_xsarm_control xsarm_control.launch.py robot_model:=px150 use_sim:=true
```

To get more details and official tutorial, please visit:[Python Demos](https://docs.trossenrobotics.com/interbotix_xsarms_docs/ros2_packages/python_demos.html)

# interbotix_xsarm_moveit
This package is used for control the manipulator using moveit.

To run this package on the physical robot, connected the manipulator and then enter the command below in a terminal.
```console
ros2 launch interbotix_xsarm_moveit xsarm_moveit.launch.py robot_model:=px100 hardware_type:=actual
```

If running this package on a robot simulated in Gazebo Classic, enter the command below in a terminal.
```console
ros2 launch interbotix_xsarm_moveit xsarm_moveit.launch.py robot_model:=rx200 hardware_type:=gz_classic
```


If running this package on a MoveIt generated fake robot, enter the command below in a terminal.
```console
ros2 launch interbotix_xsarm_moveit xsarm_moveit.launch.py robot_model:=wx250 hardware_type:=fake
```

To get more details and official tutorial, please visit:[MoveIt 2 Motion Planning Configuration](https://docs.trossenrobotics.com/interbotix_xsarms_docs/ros2_packages/moveit_motion_planning_configuration.html)

# python demos
python demo 1

<video width="320" height="240" controls>
    <source src="[demo1.mp4](https://github.com/Team-7-UOM/Manipulator-Control/blob/main/demo1.mp4)" type="video/mp4">
</video>
