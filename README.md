# Autonomous Targeting System (ATS)
## MAE 148 Final Project
### Team 11 Fall 2025

## Team Members
- Matthew Hwang - Mechanical Engineering
- Andrea Galliano - Aerospace Engineering
- David Quan - Mechanical Engineering
- Jose Umana -  Electrical Engineering 

(insert an image of our car)
(insert image of JSOE and UCSD logos somewhere as well)

## Abstract
The goal of this project is to develop a targeting system using OpenCV that scans, labels, and locks onto targets of interest, then allows for manual selection of a target. 
A two degree-of-freedom (DOF) gimbal mechanism accurately follows the selected target to keep it in frame at all times, constantly ready to fire a rocket engine.

## What We Delievered
- OpenCV with OAK-D camera for objection detection and tracking
- Dual servo motor control for object following
- Target selection system

## Nice to Haves
- Implementing created rockets engines  
- LIDAR and/or OAK-D camera depth mechanisms to access objects as potential targets from far away 
- Adding an autonomous driving feature to allow the ATS to access and be within accurate firing distance of objects out of range
- Integration of prototyped ignition system for firing rocket engines

## Demonstration (Video)




https://github.com/user-attachments/assets/16eb97ce-2f67-4ed8-98f5-33ec005cf2fc
## Smart-Cam Feature
- A feature that was added to increase efficiency and effectiveness of our project was our Smart-Cam implementation. Smart-Cam enables our PID ontrolled gimbal to move the camera in response to a moving target. The speeds of the tracking can be adjusted within the pythoon scripts. Additionally, Smart-Cam is able to recall the direction a target was before it left the field of view of the camera. By recalling this information, it is able to make smart decisions such as automatically scanning for the object again in the direction of where the target has last left.

## Mode Explanations
- Mode 1 [Scan Surrounding]: Gimbal pans 180 degreees horizontally to look for targets. If a potential target is found, the system will take 3 seconds to the object as a target in order to avoid false detections. After a target is registered, the target will have a number ID, their stationary position is registered, and their hitbox will turn yellow.
  
- Mode 2 [Choose Target]: Once a target is registered from mode 1, the user can manually lock on a target based on their remembered position. Their target ID can be pressed and the gimbal will instantly center to camera towards the desired target.

- Mode 3 [Fire Rocket]: Before the fire command is used, a target should be chosen from mode 2. When the fire command is pressed, a 5 second countdown will begin on the top right corner. Once the countdown reaches 0, their hitbox turns red. This mode represents when our created ignition system would have activated to fire our rocket engine at the desired target.

## CAD Model Assemblies
- Final Car Assembly
<img width="621" height="491" alt="FinalAssemblySetup" src="https://github.com/user-attachments/assets/223e0eef-5dad-4fe7-b09d-e404ce696717" />

- Initial Car Assembly
<img width="827" height="584" alt="EarlyQuarterSetup" src="https://github.com/user-attachments/assets/3c7b90da-147a-4233-a5c1-3a7fbd690cf8" />

## Ignition Systems Schematic
<img width="593" height="396" alt="Ignition system" src="https://github.com/user-attachments/assets/844c7042-6406-4b19-8649-8dae65aab2ba" />

## Electric Diagram
<img width="727" height="414" alt="electrical diagram" src="https://github.com/user-attachments/assets/838ac5c9-671a-4e54-a26b-feed91f9b829" />
al 
