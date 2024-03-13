# Manipulator-Control
This repository contains packages for controlling the manipulators

# interbotic_xsarm_control
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
