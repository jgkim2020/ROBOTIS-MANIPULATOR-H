# ROBOTIS MANIPULATOR-H
![](http://emanual.robotis.com/assets/images/platform/manipulator/manipulator_product.gif)

## Quick tutorial on gazebo (2019.02.28)
- Prerequisite (your mileage may vary)

  sudo apt-get install ros-kinetic-qt-build
  
  sudo apt-get install ros-kinetic-dynamixel-sdk

- Following packages must be built with catkin_make (~/catkin_ws/src/)
  
  ROBOTIS-MANIPULATOR-H
  
  ROBOTIS-Framework
  
  ROBOTIS-Framework-msgs
  
  ROBOTIS-Math
  
  DynamixelSDK

- Simple example from official ROBOTIS docs

  https://github.com/ROBOTIS-GIT/emanual/blob/master/docs/en/platform/manipulator_h/manipulator_ros.md#overview-6

  https://github.com/ROBOTIS-GIT/ROBOTIS-MANIPULATOR-H

- Step-by-step procedure
  
  **roscore**
  
  **roslaunch manipulator_h_gazebo manipulator_h_gazebo.launch**
  
    *Press the play button in gazebo to start clock*
  
  **roslaunch manipulator_h_manager manipulator_h_manager_gazebo.launch**
	  
    *Can’t control the robot without this node*
  
  **rosrun manipulator_h_gui manipulator_h_gui**
    
    *Press ‘Set Mode’ to enable robot controls*
  
- Topics of interest

  /robotis/base/set_mode_msg
  
	/robotis/base/joint_pose_msg

- Misc.

  Some issues with publishing topics when using python (C++ is preferred)

## ROS Packages for ROBOTIS MANIPULATOR-H 

|Version|Kinetic + Ubuntu Xenial|Melodic + Ubuntu Bionic|
|:---:|:---:|:---:|
|[![GitHub version](https://badge.fury.io/gh/ROBOTIS-GIT%2FROBOTIS-MANIPULATOR-H.svg)](https://badge.fury.io/gh/ROBOTIS-GIT%2FROBOTIS-MANIPULATOR-H)|[![Build Status](https://travis-ci.org/ROBOTIS-GIT/ROBOTIS-MANIPULATOR-H.svg?branch=kinetic-devel)](https://travis-ci.org/ROBOTIS-GIT/ROBOTIS-MANIPULATOR-H)|-|

## ROBOTIS e-Manual for ROBOTIS MANIPULATOR-H
- [ROBOTIS e-Manual for ROBOTIS MANIPULATOR-H](http://emanual.robotis.com/docs/en/platform/manipulator_h/introduction/)

## Wiki for manipulator_h Packages
- http://wiki.ros.org/manipulator_h (metapackage)
- http://wiki.ros.org/manipulator_h_base_module
- http://wiki.ros.org/manipulator_h_base_module_msgs
- http://wiki.ros.org/manipulator_h_bringup
- http://wiki.ros.org/manipulator_h_description
- http://wiki.ros.org/manipulator_h_gazebo
- http://wiki.ros.org/manipulator_h_gui
- http://wiki.ros.org/manipulator_h_kinematics_dynamics
- http://wiki.ros.org/manipulator_h_manager

## Open Source related to ROBOTIS-MANIPULATOR-H
- [manipulator_h](https://github.com/ROBOTIS-GIT/ROBOTIS-MANIPULATOR-H)
- [rh_p12_rn](https://github.com/ROBOTIS-GIT/RH-P12-RN)
- [robotis_framework](https://github.com/ROBOTIS-GIT/ROBOTIS-Framework)
- [robotis_controller_msgs](https://github.com/ROBOTIS-GIT/ROBOTIS-Framework-msgs)
- [robotis_math](https://github.com/ROBOTIS-GIT/ROBOTIS-Math)
- [dynamixel_sdk](https://github.com/ROBOTIS-GIT/DynamixelSDK)

## Documents and Videos related to ROBOTIS-MANIPULATOR-H
- [ROBOTIS e-Manual for ROBOTIS MANIPULATOR-H](http://emanual.robotis.com/docs/en/platform/manipulator_h/introduction/)
- [ROBOTIS e-Manual for RH-P12-RN](http://emanual.robotis.com/docs/en/platform/rh_p12_rn/)
- [ROBOTIS e-Manual for ROBOTIS Framework](http://emanual.robotis.com/docs/en/software/robotis_framework_packages/)
- [ROBOTIS e-Manual for Dynamixel SDK](http://emanual.robotis.com/docs/en/software/dynamixel/dynamixel_sdk/overview/)
