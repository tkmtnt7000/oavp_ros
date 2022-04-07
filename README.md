# Omni Audio Visual Package

[![main](https://github.com/tkmtnt7000/oavp_ros/actions/workflows/main.yaml/badge.svg)](https://github.com/tkmtnt7000/oavp_ros/actions/workflows/main.yaml)

This is the package for using a set of omni directional camera, speaker and mic by ROS.

## Create standalone workspace
```bash
mkdir ~/catkin_ws/src -p
cd ~/catkin_ws/src
git clone https://github.com/tkmtnt7000/oavp_ros.git
wstool init .
wstool merge oavp_ros/oavp.rosinstall
wstool update
rosdep update
rosdep install -y -r --from-paths . --ignore-srd
source /opt/ros/$(ROS_DISTRO}/setup.bash
catkin init
catkin build oavp_ros
```

## Usage
```bash
roslaunch oavp_ros oavp.launch
```
