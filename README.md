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

<img width="923" alt="Screenshot 2021-10-10 at 3 01 05 PM" src="https://user-images.githubusercontent.com/31934929/136698929-a0e37d73-89d1-44be-9dca-b0aaff734899.png">


Rviz initial stage of localization 

<img width="787" alt="Screenshot 2021-10-10 at 1 50 23 PM" src="https://user-images.githubusercontent.com/31934929/136698894-5357964a-96f7-4954-845a-7f617854b80e.png">

Converging to a good solution

<img width="771" alt="Screenshot 2021-10-10 at 2 04 31 PM" src="https://user-images.githubusercontent.com/31934929/136698909-5375a903-4356-4641-a6d7-7995b0061591.png">

