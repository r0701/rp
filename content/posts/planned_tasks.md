---
title: Planned Tasks
date: 2019-09-25T05:00:45.000+00:00

---
## UAV search and Pursuit other UAV in motion

 1. \[X\] UAV autonomous vertical takeoff to a specific altitude
 2. \[X\] UAV autonomous landing from current altitude
 3. \[X\] UAV navigate from current position to a specific position using the shortest path with collision avoidance (GPS coordinates)
 4. \[X\] UAV hovering and visual ground mapping at a specific altitude and executing a specific trajectory (path is a 3D coordinate function)
 5. \[X\] UAV autonomous search for the target
 6. \[X\] UAV attention on a target (visual tracking) by controlling:
 7. \[ \] UAV intercepts a target in the air
 8. \[ \] UAV clamps/hooks a target in the air
 9. \[ \] UAV releases a target into a box in the ground
10. \[ \] UAV challange 1 trials

### What we can do

Discussion for task number:

1. Drone can fly to a given altitude
2. Drone can land in a given coordinate
3. Drone can navigate to a goal coordinate while avoiding obstacles 
4. Drone can map the ground and use it to calculate the shortest path
5. Drone can fly to a given height and hovers until a target is found
   1. tools: ROS darknet
6. Drone uses an algorithm to keep the object centered in the view, once lost the drone initiates another algorithm to locate the target again

***

## Scenario

Two UAVs: One searches for the target and the second captures the target.

1. Drone 1 flies to a given altitude
2. Searches for a target
3. Keeps the target in view, estimate the coordinate of the target (depth, not completed yet)
4. Sends target coordinate to  Drone 2
5. Drone 2 goes to target
6. Captures the ball and returns home (capturing mechanism not defined yet) 