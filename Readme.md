## ROS Pub-Sub Project 2024

## How to run 

- in the root of the project [ros_ws] check for missing dependencies before building
```sh
rosdep install -i --from-path src --rosdistro humble -y
```
- in the root [ros_ws] build the package
```sh
colcon build --packages-select py_pubsub
```
- Open a new terminal navigate to  [ros_ws] and source the setup files
```sh
source install/setup.bash
```
- Now run the talker node:
```sh
ros2 run py_pubsub talker
```
- Now Open a new terminal navigate to [ros_ws] and source the setup files
```sh
source install/setup.bash
```
- And then start the listener node
```sh
ros2 run py_pubsub listener
```
