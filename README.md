# ros_localization
This repository analyses the amcl package to localize a robot with hokuyo LIDAR and odometry readings.

## How to Run
1) Install the ros AMCL(adaptive monte carlo localization) package, if not already installed.
2) clone the github packages to your catkin workspace.
3) Launch the gazebo world, rviz and wheeled robot using $roslaunch my_robot world.launch
4) start the map server for amcl package and load the map created using pgm_map_creator. $rosrun map_server map_server {specify path}/map.yaml
5) start the acml package using the launch file provided. $roslaunch my_robot acml.launch
6) Finally start the teleop paackage to control the robot. $rosrun teleop_twist_keyboard teleop_twist_keyboard.py

## Snapshots

Gazebo world 

