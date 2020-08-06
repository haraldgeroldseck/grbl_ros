# grbl_ros ![ROS 2 CI](https://github.com/flynneva/grbl_ros/workflows/ROS%202%20CI/badge.svg)

A simple ROS2 package for interfacing with a [grbl device](https://github.com/gnea/grbl).

Currently supports:
- polling status of grbl device
- sending plain GCODE commands using ROS2 service

## Supported Platforms
**All Tier 1 platforms = Windows 10, Mac OS X**

OS           | ROS 2 Version | 
------------ | ------------- | 
All Tier 1 platforms | [Dashing Diademata](https://index.ros.org/doc/ros2/Releases/Release-Dashing-Diademata/) | 
All Tier 1 platforms | [Eloquent Elusor](https://index.ros.org/doc/ros2/Releases/Release-Eloquent-Elusor/) | 
All Tier 1 platforms | [Foxy Fitzroy](https://index.ros.org/doc/ros2/Releases/Release-Foxy-Fitzroy/) | 

## Getting started

Quick start:
```bash
# for Ubuntu
sudo apt install ros-<your-distro>-grbl-ros
```

From source:
```bash
# if you use ssh
git clone git@github.com:flynneva/grbl_ros.git
# if you dont
git clone https://github.com/flynneva/grbl_ros.git
```

Once cloned, you can now build your workspace by running the following from your workspace's root directory:
```bash
colcon build
```

## TODO
Here is a list of potential ideas/features this package could have. Eventually the plan is to add all of these.
- full grbl command support & descriptions (non-modal commands, motion modes, etc.)
- safety features that grbl already implements to be translated to ROS (door sensor, estop, endstop, etc.)
- full file gcode streaming to grbl device
- publish tf of grbl machine coordinates
- ROS services for jog control
- im sure there are more but I cant think of them right now
