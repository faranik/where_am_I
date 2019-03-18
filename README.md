# where_am_I
This project is part of the *Robotics Software Engineering* scholar course offered at Udacity. It explores AMCL algorithm for the robot localization problem and its ROS node implementation. 

## Project Overview
Welcome to the Where Am I? localization project! In this project, you will learn to utilize ROS AMCL package to accurately localize a mobile robot inside a map in the Gazebo simulation environments.

Several aspects of robotic software engineering with a focus on ROS are used:

* Create a ROS package that launches a custom robot model in a custom Gazebo world.
* Utilize the ROS AMCL package and the Tele-Operation / Navigation Stack to localize the robot.
* Explore, add, and tune specific parameters corresponding to each package to achieve the best possible localization results.

## Development environment setup
If you are working with a native ROS installation or using a VM, some of the following package might need to be installed. You could install them as shown below:
```
$ sudo apt-get install ros-kinetic-navigation
$ sudo apt-get install ros-kinetic-map-server
$ sudo apt-get install ros-kinetic-move-base
$ sudo apt-get install ros-kinetic-amcl
```

## Teleop Package
If you prefer to control your robot to help it localize itself, you would need to add the teleop node. You could use ros-teleop package to send command to the robot using keyboard or controller.

Clone the ros-teleop package to your src folder:
```
cd /home/workspace/catkin_ws/src
git clone https://github.com/ros-teleop/teleop_twist_keyboard
```
Build the package and source the setup script:
```
cd ..
catkin_make
source devel/setup.bash
```
Now you could run the teleop script as is described in the README file:
``
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
