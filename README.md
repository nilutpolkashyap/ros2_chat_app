# ros2_chat_app

1. To build this package, you either need a ROS 2 workspace or create a new one. Here is the instructions to create a new ROS 2 workspace, build the package and run the instances of chat app

```
mkdir -p ~/ros2_ws/src

cd  ~/ros2_ws/src

git clone https://github.com/nilutpolkashyap/ros2_chat_app

cd ~/ros2_ws

colcon build

source install/setup.bash
