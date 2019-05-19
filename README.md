# husky_simulation_jade
Especially for Running Husky Gazebo Simulation in ROS Jade

## Syste Setup
- Ubuntu 14.04
- ROS Jade
- Gazebo 6.6

## Introduction
- Original `husky` packages from https://github.com/husky did not maintenance well in ROS jade and several packages are deprecated and merged into another package.
- `LMS1xx` package is a laser package which could be installed by `apt-get install`, but the current bug related to `robot_namespace` was just fixed (https://github.com/clearpathrobotics/LMS1xx/commit/8fae998a9df93a3fe0b287ae1d2a4f0e32abeac5), so in this repository we simply copy the fixed files into `LMS1xx` folder.
- Due to the system using Gazebo 6.6, we could not install the `ros-gazebo` related packages to manager the control between Gazebo and ROS. So we clone the original package in jade-level form https://github.com/ros-simulation/gazebo_ros_pkgs/tree/jade-devel.

## Usage
- Setup a new workspace
- Clone all this repository
- `catkin_make` as usual.
- Following the tutorial `https://www.clearpathrobotics.com/assets/guides/ros/` to enjoy more interesting demos.
