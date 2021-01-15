Step 1: Installing prerequisites:

Install git clones `turtlebot3`, `turtlebot3_msgs` and `turtlebot_simulations.git`.
```
cd ~/catkin_ws/src/
git clone https://github.com/ROBOTIS-GIT/turtlebot3.git
git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git
git clone -b kinetic-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
 cd ~/catkin_ws
catkin_make
```

To start a turtlebot 3 gazebo simulation in the given `turtlebot3_empty_world` launch file. The system expects the turtlebot3 model to be defined before running the simulation, the model can be exported before or the default model can be changed in the `turtlebot3_empty_world.launch` file.
```
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch
```

roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
