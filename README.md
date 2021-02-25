# turtlebot2_rplidar
Turtlebot2 simulation with RPLidar and a RGBD camera

## Dependancies

### Install gazebo dependancies
```
sudo apt-get install ros-melodic-gazebo-ros
sudo apt-get install ros-melodic-gazebo-plugins
sudo apt-get install pyqt5-dev-tools
```
### Install melodic dependancies
```
sudo apt-get install ros-melodic-xacro
sudo apt-get install ros-melodic-ecl-*
sudo apt-get install ros-melodic-joy
sudo apt-get install ros-melodic-yocs-controllers 
sudo apt install ros-melodic-yujin-ocs

sudo apt-get install ros-melodic-rqt-plot 
sudo apt-get install ros-melodic-robot-state-publisher
sudo apt-get install ros-melodic-rqt-robot-dashboard

```

### Install Turtlebot dependancies

```
sudo apt-get install libusb-dev
sudo apt-get install libftdi-dev
```

### Clone to ROS Workspace
```
mkdir -p ros_ws/src
cd ros_ws/src
git clone --single-branch --branch melodic https://github.com/yujinrobot/kobuki.git
git clone --single-branch --branch melodic https://github.com/yujinrobot/kobuki_msgs.git
git clone --single-branch --branch melodic https://github.com/yujinrobot/kobuki_core.git
git clone --single-branch --branch melodic https://github.com/turtlebot/turtlebot.git 
git clone --single-branch --branch melodic https://github.com/yujinrobot/kobuki_desktop.git

git clone https://github.com/arjunskumar/turtlebot2_rplidar.git

cd .. && catkin_make
```

### Launch the Turtlebot2 in Gazebo
```
source devel/setup.bash
roslaunch turtlebot2_rplidar_gazebo turtlebot_world.launch
```

![Gazebo](/img/turtlebot_gazebo.png)


If following error occurs

```[Err] [REST.cc:205] Error in REST request``` 

Change the url to  `url: https://api.ignitionrobotics.org` inside `~/.ignition/fuel/config.yaml` file

