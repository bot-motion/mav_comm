cmake_minimum_required(VERSION 3.5.0)
project(mav_msgs)


find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)
find_package(builtin_interfaces REQUIRED)

find_package(std_msgs)
find_package(geometry_msgs)
find_package(trajectory_msgs)
find_package(Eigen3)


set(msg_files
  "msg/AttitudeThrust.msg"
  "msg/RateThrust.msg"
  "msg/RollPitchYawrateThrust.msg"
  "msg/TorqueThrust.msg"
  "msg/Actuators.msg"
  "msg/Status.msg"
  "msg/FilteredSensorData.msg"
  "msg/GpsWaypoint.msg"
  )

rosidl_generate_interfaces(${PROJECT_NAME}
  ${msg_files}
)

ament_export_dependencies(rosidl_default_runtime)

ament_package()


