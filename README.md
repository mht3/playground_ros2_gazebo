# playground_ros2_gazebo
Playground test environment using ROS2 and Gazebo

Running on Ubuntu 20.04, ROS2 Foxy

Follow installation guide:

```
https://docs.ros.org/en/foxy/Installation/Ubuntu-Install-Debians.html
```

Each time a terminal is opened, run this command to activate ROS2 Foxy

```
source /opt/ros/foxy/setup.bash
```

Check ROS2 Foxy is the correct distrubution.

```
printenv ROS_DISTRO
```

Download necessary ros2-gazebo packages

```
sudo apt install ros-foxy-gazebo-ros-pkgs ros-foxy-cartographer ros-foxy-cartographer-ros ros-foxy-navigation2 ros-foxy-nav2-bringup

```
Download necessary turtlebot3 packages

```
sudo apt install ros-foxy-turtlebot3-msgs ros-foxy-dynamixel-sdk ros-foxy-hls-lfcd-lds-driver
```

Create turtlebot workspace and clone turtlebot repo into src directory.

```
mkdir -p turtlebot_3_ws/src
cd turtlebot_3_ws/src
git clone -b foxy-devel https://github.com/ROBOTIS-GIT/turtlebot3
git clone -b foxy-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations
```

Build Downloaded Packages

```
cd ../
```
