cmake_minimum_required(VERSION 3.0.2)
project(omni_learning)

## Compile as C++11, supported in ROS Kinetic and newer
add_compile_options(-std=c++11)

find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  nav_msgs
  roscpp
  rospy
  std_msgs
)

catkin_package()

include_directories(${catkin_INCLUDE_DIRS})

catkin_install_python(PROGRAMS
  src/dqn_node.py
  src/result_graph.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)