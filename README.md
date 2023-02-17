# JLR_Robotic_Charging

<!-- PROJECT DESCRIPTION -->

## Introduction:
The objective of this project was to develop a robotic arm that can automatically detect the vehicle's charging port and plug the socket into the charging port.

## Methodology:
<p>◦The CAD model of the robotic arm was developed using Fusion360 and SolidWorks. The Robotic arm simulation was done on MATLAB using the Kinova Gen3 Model for testing arm control algorithms.</p>
<p>◦For perception, a Yolov7 model was trained to detect the CCS2 charging port. Then, stereo cameras were used to determine the distance to the charding port. Finally an Aruco marker placed near the charging port was used to obtain the 6D pose.</p>
<p>◦For the given end pose, we create an inverse kinematics solver. To solve the inverse kinematics for each waypoint, we first obtain the target pose as a function of the waypoints and their orientations. The joint waypoints are then defined via the inverse kinematics function.</p>
<p>◦We have defined 4 ways to generate a trajectory, namely ‘trap’, ‘cubic’, ‘quintic’, and ‘bspline’</p>
<p>◦Then, we plot Velocity vs Time, Acceleration vs Time, Torque vs Time and Power vs Time via which we can find average power.</p>
<p>◦Torque is defined using the inverseDynamics function with the pose, velocity, acceleration and external forces as variables.</p>
<p>◦We finally visualize the robotic arm motion on a 3D plot</p>


## Robot Arm Design:

Objective:
To design a robotic arm that should be able to reach the charging port of the electric vehicle from the charging station with all the constraints as stated

Approach:
Two different approaches have been taken to achieve the said objective
Design_1: Design of a 6-DOF robotic arm 
Design_2 (alternate approach): Design of a 6-DOF robotic arm using pneumatically controlled artificial muscles for tough robotic applications

Design Specifications:
DOF: 6
Mass: 54.2 kg
Bounding box dimension: 0.16*0.7*0.17 (m)
Payload: 5 kg
Max. reach: 1.42 m
Material: Al 6061 T6, PLA (3D printed shells for motor casing)

## Bill of Materials
<p align="center">
  <img src="https://github.com/AdityaGuhagarkar/JLR_Robotic_Charging/Bill of Material/BOM.png" width="350" title="">
</p>

## Plots
<p align="center">
  <img src="https://github.com/AdityaGuhagarkar/JLR_Robotic_Charging/plots/plot1.jpg" width="350" title="">
</p>
<p align="center">
  <img src="https://github.com/AdityaGuhagarkar/JLR_Robotic_Charging/plots/plot2.jpg" width="350" title="">
</p>

## Conclusion:
The project was successful in designing a inexpensive Robotic Arm that can obtain the 6D pose of a CCS2 charging port and travel to a given 6D pose with the optimal trajectory. The breakthrough of the project was use the comparison of multiple trajectories to determine the most optimized one. In terms of the design the use of Pneumatic Artificial Muscles in the robotic arm end-effector is a major brakthrough as it is in-expensive and can carry 10 to 20 times the weight of a normal robotic hand.

## Installations
1) Install the MATLAB 2022b software
2) Download Fusion360 or SolidWorks to open the CAD model
3) ROS noetic

## Steps to run the code
1) Download the Robtic_Arm_Team53.mlx file and run it on the MATLAB 2022b software

## Contact Us

**Aditya Guhagarkar:**
[![](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aditya-guhagarkar/)
[![](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AdityaGuhagarkar)
[![](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:adityaguhagarkar@gmail.com)

