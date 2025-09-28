# ROS 2 in Docker

This repository provides a Docker environment for running ROS 2 Humble.  
It allows you to develop and test ROS 2 applications without installing ROS 2 directly on your host system.

---

## 🚀 Getting Started

### 1. Build the Docker image
From the root of this repo, run:

```bash
docker build -t ros2:humble_ws .

2. Run the container

Mount a local workspace folder (~/my_ros_projects) into the container’s /root/ros2_ws:

```bash
docker run -it -v ~/my_ros_projects:/root/ros2_ws ros2:humble_ws

This opens a shell inside the container with ROS 2 installed.

3. Verify ROS 2 installation

Inside the container, check versions to verify installation:

ros2 --help
colcon --help


