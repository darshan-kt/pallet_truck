cmake_minimum_required(VERSION 2.8.3)
project(pallet_truck_gazebo)


find_package(catkin REQUIRED
    roscpp
    std_srvs
    std_msgs
    tf
    gazebo_ros
)

catkin_package()


install(DIRECTORY launch worlds models rviz
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})


