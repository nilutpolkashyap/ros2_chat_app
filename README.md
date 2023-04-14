# ros2_chat_app

# To build the code:

1. To build this package, create a new ROS 2 workspace, build the package and run the instances of chat app

```
mkdir -p ~/ros2_ws/src

cd  ~/ros2_ws/src

git clone https://github.com/nilutpolkashyap/ros2_chat_app

cd ~/ros2_ws

colcon build

source install/setup.bash
```

# To run the code

Open 2 new terminals. Execute following commands in the corresponding terminal

Terminal 1:
```
cd ~/ros2_ws
source install/setup.bash
ros2 run ros2_chat_app chat_app --ros-args --remap __node:=chat_node_1 -p send_topic:=chat1 -p  recv_topic:=chat2

```
Terminal 2:

```
cd ~/ros2_ws
source install/setup.bash
ros2 run ros2_chat_app chat_app --ros-args --remap __node:=chat_node_2 -p send_topic:=chat2 -p  recv_topic:=chat1
```
