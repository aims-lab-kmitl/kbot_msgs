cmake_minimum_required(VERSION 3.0.2)
project(kbot_msgs)

find_package(catkin REQUIRED COMPONENTS
    std_msgs
    message_generation
)

################################################
## Declare ROS messages, services and actions ##
################################################

add_message_files(
  FILES
  lowlevel.msg
  pid.msg
)

generate_messages(
  DEPENDENCIES
  std_msgs
)

################################################
## Declare ROS dynamic reconfigure parameters ##
################################################

###################################
## catkin specific configuration ##
###################################

catkin_package(
 CATKIN_DEPENDS std_msgs message_runtime
)

###########
## Build ##
###########

#############
## Install ##
#############

#############
## Testing ##
#############
