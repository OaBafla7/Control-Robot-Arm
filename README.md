
# ROS2 Robot Arm Control Project

## Project Overview
This project demonstrates how to control a robotic arm using ROS2. It includes joint control, and integration with ROS2 Control and  Rviz.

## Prerequisites

### System Requirements
- Ubuntu 22.04 (recommended)
- ROS2 Humble installation
- Basic programming knowledge (Python/C++)

### ROS2 Packages Installation
```bash
sudo apt-get update && sudo apt-get install -y \
    ros-humble-joint-state-publisher-gui \
    ros-humble-gazebo-ros \
    ros-humble-xacro \
    ros-humble-ros2-control \
    ros-humble-ros2-controllers \
    ros-humble-joint-state-broadcaster \
    ros-humble-joint-trajectory-controller \
    ros-humble-controller-manager \
    ros-humble-moveit \
    ros-humble-gazebo-ros2-control
```

## Installation Guide

1. Clone the repository to your ROS2 workspace:
```bash
cd ~/ros2_ws/src
git clone https://github.com/smart-methods/Robot_Arm_ROS2.git
```

2. Build the project:
```bash
colcon build
```

3. Source the workspace:
```bash
. install/setup.bash
```

## Usage Instructions

### Launching the Robot Visualization
To visualize and control the robot arm using the joint state publisher:
```bash
ros2 launch arduinobot_description display.launch.py
```

### Key Features
1. **Joint Control**: Interactive sliders for each joint
2. **Gazebo Simulation**: Realistic physics simulation
3. **ROS2 Control**: Hardware abstraction layer
4. **MoveIt Integration**: Motion planning capabilities

## Project Structure
```
Robot_Arm_ROS2/
├── config/            # Configuration files
├── launch/            # Launch files
├── meshes/            # 3D model assets
├── rviz/              # RViz configuration
├── src/               # Source code
├── urdf/              # URDF/XACRO files
└── worlds/            # Gazebo world files
```

## Screenshots
![Robot Visualization](https://github.com/user-attachments/assets/593be3b5-e5a6-4b6f-9dce-a3aad6a18cd4)
![Gazebo Simulation](https://github.com/user-attachments/assets/470bae45-781b-4a07-b52a-fe463808fe28)

## Troubleshooting

### Common Issues
1. **Missing Dependencies**:
   ```bash
   rosdep install --from-paths src --ignore-src -r -y
   ```

2. **Build Errors**:
   - Ensure all dependencies are installed
   - Clean build and rebuild:
     ```bash
     rm -rf build install log
     colcon build
     ```

3. **Launch File Issues**:
   Verify package names in launch files match your workspace structure


---


