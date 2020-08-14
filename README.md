# turtlebot2_rplidar
ROS simulation package for Turtlebot2 with RPLidar and a RGBD camera

## Dependancies

### Depandancies for real robot

```
sudo apt-get install libusb-dev
sudo apt-get install libftdi-dev
```
### Install gazebo dependancies
```
sudo apt-get install ros-melodic-gazebo-ros
sudo apt-get install ros-melodic-robot-state-publisher
```
### Install melodic dependancies
```
sudo apt-get install ros-melodic-xacro
sudo apt-get install ros-melodic-ecl-exceptions
sudo apt-get install ros-melodic-ecl-geometry
sudo apt-get install ros-melodic-ecl-threads
sudo apt-get install ros-melodic-ecl-mobile-robot
sudo apt-get install ros-melodic-ecl-devices
sudo apt-get install ros-melodic-ecl-sigslots
sudo apt-get install ros-melodic-ecl-command-line
sudo apt-get install ros-melodic-ecl-streams
sudo apt-get install ros-melodic-joy
sudo apt-get install ros-melodic-yocs-controllers 
sudo apt install ros-melodic-yujin-ocs
```

### Create ROS Workspace
```
mkdir -p ros_ws/src
cd ros_ws/src
git clone --single-branch --branch melodic https://github.com/yujinrobot/kobuki.git
git clone --single-branch --branch release/0.7-melodic https://github.com/yujinrobot/kobuki_msgs.git
git clone --single-branch --branch melodic https://github.com/yujinrobot/kobuki_core.git
git clone --single-branch --branch melodic https://github.com/turtlebot/turtlebot.git 
```
