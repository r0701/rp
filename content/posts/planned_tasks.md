---
title: Planned Tasks
date: 2019-09-25T05:00:45.000+00:00

---
## UAV search and Pursuit other UAV in motion

1. UAV autonomous vertical takeoff to a specific altitude
2. UAV autonomous landing from current altitude
3. UAV navigate from current position to a specific position using the shortest path with collision avoidance (GPS coordinates)
4. UAV hovering and visual ground mapping at a specific altitude and executing a specific trajectory (path is a 3D coordinate function)
5. UAV autonimous search for the target: 
     - A UAV in the air
6. UAV attention on a target (visual tracking) by controlling:
     - visual pursuit (control distance to target)
7. UAV intercepts a target in the air
8. UAV clamps/hooks a target in the air
6. UAV releases a target into a box in the ground
3. UAV challange 1 trials

### What we can do

- We can do Tasks 1, 2 and most of 3.

- Task 1 and 2 can be done using one command which makes the drone fly to a certain altitude then back down to the starting position. This can be done using more than one method: We can use the package made by Pedro and his team which gives a set of coordinates for the drone to follow, moving to the next whenever it gets within range of the prior point. Task 2 can be done by giving the drone a command to land or by giving the drone a coordinate of (0,0,0) x,y,z coordinates.

- We can navigate to a position but we have no way to view an obstacle yet, hence, we cannot do the collision avoidance but we can go to a certain coordinate as explained above.

- Task 4 can be done, partially, by using the inbuilt camera mapping sequence provided either by ZED or Intel's T265 camera. These methods my prove to be inadequate for mapping large areas.