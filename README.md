# RoboticsND: Project #2
This repository contains the files for Udacity's Robotics Nanodegree's Second Project

Find Udacity's Robotics Software Engineering Nanodegree [here](https://www.udacity.com/course/robotics-software-engineer--nd209).

## Project Requirements

- Design a differential drive robot using URDF with a camera and a LIDAR sensor
- Create a new world environment in Gazebo
- Create a custom robot ROS package to hold the robot, a white ball, and the world
- Create a `ball_chaser` ROS package to hold all C++ nodes
- Write a `drive_bot` C++ node that will provide a ball_chaser/command_robot service to drive the robot by controlling its linear x and angular z velocities
- Write a `process_image` C++ node that reads your robot’s camera image, analyzes it to determine the presence and position of a white ball

<!-- The requirements of this project were met as approved by Udacity's reviewers. -->

## Design Process

- Designed a differential drive robot using Solidworks (STLs available inside `drive_bot/meshes`) then exported it to URDF using [Solidworks to URDF Exporter](https://github.com/ros/solidworks_urdf_exporter)
- Tweaked URDF to fix axis and coordinate systems, added camera and LIDAR sensor to robot model
- Designed a maze world using Gazebo's Building Editor based on [this maze](https://www.researchgate.net/figure/Sample-maze-used-in-computer-simulations_fig6_315969093)
- Wrote C++ nodes `drive_bot` and `process_image` to drive the robot's wheels based on the position of the white ball as obtained by the latter node
- Packaged launching into a single launch file for each of the ROS packages


## Screenshots

Find the following images showing the a few details of the project.

![](https://i.imgur.com/Le9zi2a.jpg)
<p align = "center"><b>Fig.1 - Solidworks Render of Robot Model</b></p>
<br />

![](https://i.imgur.com/xWLBBJS.png)
<p align = "center"><b>Fig.2 - Close Up View of Robot Model in Gazebo</b></p>
<br />

![](https://i.imgur.com/I4IoLZU.png)
<p align = "center"><b>Fig.3 - Gazebo Maze World View</b></p>
<br />

![](https://i.imgur.com/DzFbFGM.png)
<p align = "center"><b>Fig.4 - Top View of Gazebo Maze World</b></p>
<br />


## Credits

This project was fully done by myself.
