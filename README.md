# Omni Reinforcement Learning using Deep Q-network
This package implement Deep Q-network for Omni-directional mobile robot moving to target position.<br>
The Robot model is using the Omni Robot, [github](https://github.com/duynamrcv/omni_robot)
## Requirement
```
Ubuntu 20.04, Python 3.8
ROS Noetic
tensorflow
pyqtgraph
```

## Installation
```
$ pip install -upgrade tensorflow
$ pip intall pyqtgraph
```

## Prerequisite
```
$ sudo apt install ros-noetic-gazebo-ros
```

## Running
```
$ roslaunch omni_learning stage.launch
$ roslaunch omni_learning result_graph.launch
$ roslaunch omni_learning dqn.launch
```