cmake_minimum_required(VERSION 3.0.2)
project(ituauv_uuv_descriptions)

## Compile as C++11, supported in ROS Kinetic and newer
# add_compile_options(-std=c++11)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  uuv_assistants
  uuv_descriptions
  uuv_gazebo
  uuv_gazebo_ros_plugins
  uuv_sensor_ros_plugins
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES ituauv_uuv_descriptions
#  CATKIN_DEPENDS roscpp rospy uuv_assistants uuv_descriptions uuv_gazebo uuv_gazebo_ros_plugins uuv_sensor_ros_plugins
#  DEPENDS system_lib
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)