# Control-Robot-Arm
Control robot arm by joint using ROS2

Getting Started

You can decide whether to build the real robot or just have fun with the simulated one. The course can be followed either way, most of the lessons and most of the code will work the same in the simulation as in the real robot
Prerequisites

You don't need any prior knowledge of ROS 2 or of Robotics, I'll explain all the concepts as they come out and as they are needed to implement new functionalities to our robot. A basic knowledge of programming, either using C++ or Python is required as this is not a Programming course and so I'll not dwell too much on basic Programming concepts.

To prepare your PC you need:
sudo apt-get update && sudo apt-get install -y \
     ros-humble-joint-state-publisher-gui \
     ros-humble-gazebo-ros \
     ros-humble-xacro \
     ros-humble-ros2-control \
     ros-humble-ros2-controllers \
     ros-humble-joint-state-broadcaster \
     ros-humble-joint-trajectory-controller \
     ros-humble-controller-manager
     ros-humble-moveit \
     ros-humble-gazebo-ros2-control

Installation

1- Clone the repo:

cd ~/ros2_ws/src
git clone https://github.com/smart-methods/Robot_Arm_ROS2.git
colon build

Source The Project:
. install/setup.bash

Usage

Controlling the robot arm by joint_state_publisher

ros2 launch arduinobot_description display.launch.py

<img width="1208" height="712" alt="Screenshot from 2025-08-04 14-51-06" src="https://github.com/user-attachments/assets/e1139fb6-2d7c-4e3f-8fc2-055ca8f0923a" />


<img width="1208" height="712" alt="Screenshot from 2025-08-04 14-51-43" src="https://github.com/user-attachments/assets/ecfaaade-0050-4c76-8f4c-9b7347aec3ba" />


   
<img width="1208" height="712" alt="Screenshot from 2025-08-06 19-54-06" src="https://github.com/user-attachments/assets/593be3b5-e5a6-4b6f-9dce-a3aad6a18cd4" />




    
    Install ROS 2 Humble on your Ubuntu 22.04
    Install ROS 2 missing libraries. Some libraries that are used in this project are not in the standard ROS package. Install them with:
