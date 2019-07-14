# RoboND_Map_My_World
 
This the project of Udacity Robotics Software Development Nanodegree project of SLAM and Mapping. The packages used are [rtabmap_ros](http://wiki.ros.org/rtabmap_ros) and [ROS Teleop Package](https://github.com/ros-teleop/teleop_twist_keyboard).

**To review the rtabmap.db file, it is too big for github(271 MB), please use this OneDrive [link](https://uflorida-my.sharepoint.com/:u:/g/personal/wangyiqun_ufl_edu/EUbxcCs4OJBOrA978pFLavYBK5Rc41N_vap1-2NlUlknXw?e=80PlKr) to download it**

# Installation

## rtabmap_ros package install:
```bash
$ sudo apt-get install ros-kinetic-rtabmap-ros
```

## ROS Teleop Package install:
```bash
$ cd (catkin_ws)/src
$ git clone https://github.com/ros-teleop/teleop_twist_keyboard.git
$ cd ..
$ catkin_make
```
Then, try to run it:
```bash
$ cd (catkin_ws)
$ source devel/setup.bash
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
If not working:
```bash
$ cd (catkin_ws)/src/teleop_twist_keyboard
$ chmod +x teleop_twist_keyboard.py
```
Then run it again.

## Project Package install:
```bash
$ cd (catkin_ws)/src
$ git clone https://github.com/pat-CIMAR-UF/RoboND_Map_My_World.git my_robot
$ cd ..
$ catkin_make
```

# To Run
To launch the robot and world package:
```bash
$ cd (caktin_ws)
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```
To launch the teleop package to control the robot: Open a new terminal:
```bash
$ source devel/setup.bash
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
To launch the rtabmap_ros package:
```bash
$ source devel/setup.bash
$ roslaunch my_robot mapping.launch
```



