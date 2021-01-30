cmake_minimum_required(VERSION 3.5.0)
project(mav_msgs)


find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

find_package(std_msgs)
find_package(geometry_msgs)
find_package(trajectory_msgs)
find_package(Eigen3)



#rosidl_generate_interfaces(${PROJECT_NAME}
#  "msg/Actuators.msg"
#  "msg/AttitudeThrust.msg"
#  "msg/RateThrust.msg"
#  "msg/RollPitchYawrateThrust.msg"
#  "msg/TorqueThrust.msg"
#  "msg/Status.msg"
#  "msg/FilteredSensorData.msg"
#  "msg/GpsWaypoint.msg"
#)

ament_package()


