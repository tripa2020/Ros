cmake_minimum_required(VERSION 3.0.2)
project(sdf_prac)

find_package(catkin REQUIRED COMPONENTS
  gazebo
  gazebo_ros
  roscpp
  rospy
)

## Generate messages in the 'msg' folder
# add_message_files(
#   FILES
#   Message1.msg
#   Message2.msg
# )

## Generate services in the 'srv' folder
# add_service_files(
#   FILES
#   Service1.srv
#   Service2.srv
# )

catkin_package(
#  LIBRARIES sdf_prac
  DEPENDS gazebo_ros roscpp rospy
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
  ${Boost_INCLUDE_DIR}
  ${GAZEBO_INCLUDE_DIRS}
)
link_directories(${GAZEBO_INCLUDE_DIRS})

