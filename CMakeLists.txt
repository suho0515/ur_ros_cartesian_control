cmake_minimum_required(VERSION 3.0.2)
project(ur_ros_cartesian_control)

find_package(catkin REQUIRED COMPONENTS
  rospy
)

catkin_package(
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

catkin_install_python(PROGRAMS src/ur_point_node.py
                      DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})
