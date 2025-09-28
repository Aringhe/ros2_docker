---

### 📄 `VALIDATION.md`

```markdown
# ROS 2 Validation

This document explains how to validate the ROS 2 environment in Docker by running the talker/listener demo.

---

## 1. Start a container
Run the container with a mounted workspace:

```bash
docker run -it -v ~/my_ros_projects:/root/ros2_ws ros2:humble_ws

2. Run the Talker

Inside the container, in Terminal 1:


```bash
ros2 run demo_nodes_cpp talker


This will publish messages on the /chatter topic.


3. Run the Listener

Open a second terminal, attach to the same container, and run:

```bash
docker exec -it <container_id> bash

Then inside the container run:

```bash
ros2 run demo_nodes_cpp listener


4. Stopping the Demo
	•	To stop either talker or listener, press: CTRL + C


	•	To stop the whole container, type: exit (or press: CTRL + D)
