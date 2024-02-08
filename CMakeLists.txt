cmake_minimum_required(VERSION 2.8.3)
project(motor_angles_msg)

find_package(catkin REQUIRED COMPONENTS roscpp rospy message_generation std_msgs)

add_message_files(FILES
	MotorAngles.msg
)

generate_messages(DEPENDENCIES std_msgs)

catkin_package(CATKIN_DEPENDS message_runtime  std_msgs)

include_directories(${catkin_INCLUDE_DIRS})
