---
title: "Tests to perform on the 15th of October"
date: 2019-09-25T08:43:56+04:00
draft: true
---
# Tests to perform on the 15th of October

## Capturing images for training 
 - Drone
 - Ball
 - Drone with the ball
 - Method to capture images: 
     - drone carrying the ball, flying in a figure 8 (a lot of batteries)
     - multiple drones with camera capturing from all angles, also capturing multiple drones in the same view
     - on ground camera/video to capture drones flying

## Test jetson + zed camera on the drone (Hardware)

1. Test flying time
2. Test positional tracking through zed camera
3. Same for intel and realsense camera

## Autonomous testing

1. Autonomous takeoff and landing
2. Fly a specific GPS coordinate
3. Fly in a path using a 3D quadratic function

# Test Set-up 

1. Two drones
2. One jetson and another on board pc
3. One zed and one intel camera T265
4. Set up the software
 1. Ubuntu 18 or 16
 2. Ros melodic or kinetic
 3. Mavros on both
 4. (for ZED) zed wrapper and package to translate position data from the camera message to mavros so the pixhawk can see the data
 5. (realsense) same as ZED
 6. waypoint package/file

