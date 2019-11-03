---
title: "Proposed Architecture"
date: 2019-09-25T08:43:56+04:00
draft: true
---
# Proposed Architecture

## Main operating system on the drone
* Ubuntu 18.04
    * (options) Ubuntu 16
    
## Hardware (Jetson)
* Jetson Xavier
* Drone: F550
* Camera: ZED
* Wifi-card 
* FTDI board (communicates between px4 and pc)

## Hardware (Intel NUC)
* PC: Intel NUC
* Drone: F550 with PixHawk
* Camera: Intel RealSense 265
* RGB Camrea (Object Detection)
* FTDI board (communicates between pixHawk and pc)
* Ground station with GPU (for object detection) - must contain trained tracker
* Gripper/Net to capture the ball

## Packages installed on the drone (Jetson)
* ROS
* MAVROS
* ZED SDK (if zed camera is used)
* -SOFTWARE- (software to convert the different types of positional msg between ZED and px4 through ROS)
* Gripper/Net to capture the ball

## Packages installed on the drone (Intel NUC)
* ROS
* Mavros
* Realsense package (v2.2.5)
* ddynamic (dependancy for Realsense package)
* Vision-to-Mavros (converts position msg to unique px4 position msg)

## Communication protocol
* Network (2.4 Ghz)

## Detection logic
_needs additional work_

* script to identify the object
* script to navigate towards the object
* script to check if ball is captured and then go to 'home' 
