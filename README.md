# Motion Planning for Needle Steering Robot

## Overview
This is the final project for the course, **"RBE 550 - Motion Planning"** at WPI. In this project, the main goal was to develop a motion planning algorithm for a steerable needle robot built at AIM Lab, WPI. The detailed report can be found in the **"Report"** folder. 

For a quick reference, here's a brief of all that was explored and implemented from scratch:
- [MATLAB] Kinematic Modelling of the needle as a modified Bicylce model.
- [C++] Spline-based RRT and RRT* algorithms for path planning in 3D space.
- [MATLAB] Duty-cycling and CURV steering methods for trajectory planning.


---
## Results

The following figure shows the collision-free smoothened path for the needle generated using Spline-based RRT and Spline-based RRT* algorithms. The path planning algorithms were implemented in C++. 

<figure>
    <img src="src/project/media/case3.png" height="480" width="896" />
</figure>
<br>


<br>
<br>

The following visual shows the tracking of the generated path using the CURV Steering method. This was implemented in MATLAB. 

<figure>
    <img src="src/project/media/case3.gif" height="480" width="896" />
</figure>
<br>


---
## Class Diagram of Path Planning Algorithms
<figure>
    <img src="src/project/media/classDiagram.png" height="480" width="896" />
</figure>
<br>


---
## System Integration
<figure>
    <img src="src/project/media/SI.png" height="480" width="896" />
</figure>


---
## Building

To build from source, clone the latest version from this repository into your catkin workspace and compile the package using

	```bash
	$ cd catkin_workspace/src
	$ git clone https://github.com/emmanuel-logy/visual_servoing_scara.git
	$ catkin_make
	```
---
