# ROS2 Docker Workspace

This repository provides a Docker container for ROS2 (Humble) with a ready-to-use workspace.

## Features
- Ubuntu 22.04 base image
- ROS2 Humble desktop
- Colcon build tools installed
- Workspace at /root/ros2_ws

## Getting Started

1. Clone the repo:
   git clone https://github.com/<username>/ros2_docker.git
2. Build the Docker image:
   docker build -t ros2:humble_ws .
3. Run the container:
   docker run -it -v ~/my_ros_projects:/root/ros2_ws ros2:humble_ws
