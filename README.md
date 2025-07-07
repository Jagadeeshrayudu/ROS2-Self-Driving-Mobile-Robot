# Self-Driving Robot with ROS 2: Odometry & Control

This project demonstrates how to build and simulate a self-driving robot using **ROS 2**, focusing on **odometry**, **sensor fusion**, and **control systems**. It is intended for robotics enthusiasts and developers who want to gain hands-on experience with robot localization and motion.

---

## 🚀 Features

- Odometry computation using wheel encoders
- Sensor fusion with IMU and Kalman Filters
- Velocity and pose control logic
- Full simulation in Gazebo
- Code available in both Python and C++

---

## 📦 Technologies Used

- ROS 2 (Humble or Iron)
- Gazebo
- C++ / Python
- rviz2 for visualization

---

## 🛠️ Getting Started

### Prerequisites

- Ubuntu 22.04
- ROS 2 (Humble or Iron)
- Basic understanding of terminal and programming (Python/C++)

### Setup Instructions

```bash
# Clone the repository
git clone https://github.com/jagadeeshrayudu/ros2-self-driving-mobile-robot.git
cd self-driving-ros2-odometry-control/your_workspace

# Build the workspace
colcon build

# Source the workspace
source install/setup.bash

# Launch the simulation
ros2 launch your_robot_description gazebo.launch.py

# Install Required ROS Packages
```bash
sudo apt-get update && sudo apt-get install -y \
  ros-humble-ros2-controllers \
  ros-humble-gazebo-ros \
  ros-humble-gazebo-ros-pkgs \
  ros-humble-ros2-control \
  ros-humble-gazebo-ros2-control \
  ros-humble-joint-state-publisher-gui \
  ros-humble-joy \
  ros-humble-joy-teleop \
  ros-humble-robot-localization \
  ros-humble-tf-transformations

# Project Structure
```bash
📁 your_workspace/
├── src/
│   ├── robot_description/         # URDF, launch files
│   ├── robot_control/             # Control logic
│   └── robot_localization/        # Sensor fusion and Kalman filters
├── install/
├── build/
└── README.md

# Acknowledgements
TurtleBot3 packages by ROBOTIS

ROS 2 open-source community