# Introduction

This project is for our course module in Robotics Engineering. 
The project main goal is to enable a robot (TurtleBot2) to pick up an Object from a location and Transport it to another Location. **Transportation will be done with the TurtleBot2** and the **Pick & Place with Robotic Arm (PhantomX Robot Arm)**. 

It is subdivided into different parts, each group is supposed to implement is own part and at the end make a fully autonomous scenario.

<p align="center">
<img src="Materials/images/intro.JPG" width="300">
</p>

The channel is at follows:
1. Navigation
2. Mapping & Localization
3. Fine Positioning 
4. Pick & Place
5. Mapping & Localization

Our part is based on the 3rd channel (Fine Positioning). Using a Visual Servoing techniques our robot must find the position of the target autonomously.
We describe in a brief technical survey report the different methods of **Visual Servoing**. You can find the pdf here [Technical Survey Report.](https://github.com/brown4eva/RoboticsEngineeringProject_FinePositioning/tree/master/TechnicalSurveyReport)
We will describe the method in which we used in achieving the task needed for our part.

# Problem Statement
Given any location of the robot(Turtlebot2) we are to position it at a specific location known as the load area. We are to exatcly put the Turtlebot2 in a postion where the robotic arm will be able to pick the cube and place it on the Turtlebot2.

<p align="center">
<img src="Materials/images/pos2.JPG" width="300"> <img src="Materials/images/finepos.JPG" width="300"> 
</p>

# Objectives
1. Creating  a Map
2. Navigate within the map created 
3. Going to specific location 
4. Detecting and tracking the tag
5. Moving to the exact location of the tag

# Implementation
We accomplished each task of the objectives stated in order to give a solution to the **Problem Statement** . 

**Step 1 to Step 3 :** 

These were just basic steps for us since we had hand experience with this during our Bachelor year.

If this is your first time being on this **ROS** platform please follow the steps we provided and assisted videos which will help in accomplishing the first three steps ==> [Creating_Map,Navigating_&_Going_To_Specific_Location.](https://github.com/brown4eva/RoboticsEngineeringProject_FinePositioning/tree/master/Implementations) We believe you will be able to have a hand in identifying the **Problem Statement** and also having the idea we used in solving teh problem. If you are good to go then move to step 4.

**Step 4 :**

After we have now been able to have some prior knowledge on the where abouts of the robot by following the previous steps, our next step was now to go to the location needed for the loading of the object on the Turtlebot2. We did this by adapting to the method used by the ROS book volume 2 Chapter 10 using AR Tags.

We made use of the **ROS** package **ar_track_alvar**. This package can simplify a lot of the big questions and challenges that faces modern day high fidelity perception for robotic systems by the use of fiducials being **AR Tags**. In our case our problem was fine positioning which involves the field of perception.

The **AR tags** allows us to estimate their position and orientation with respect to a camera frame based off of their size in the image and their distortion. The **ar_track_alvar** library computes the projective transformations and spits out the tag’s position. We then make use of this infomation, which gives us knowlege and distance we need to make our turtlebot2 to go to.

- In order to create the marker follow the steps provided here ==> [Creating Marker](https://github.com/brown4eva/RoboticsEngineeringProject_FinePositioning/tree/master/Implementations/Creation_of_Marker)

**Video of Detection and Tracking of AR tag**


[![](http://img.youtube.com/vi/jX8nt-r6gYA/0.jpg)](http://www.youtube.com/watch?v=jX8nt-r6gYA "Detecting and Tracking Of AR tag")


**Step 5 :**

[![](http://img.youtube.com/vi/xY6Oxkhd12M/0.jpg)](http://www.youtube.com/watch?v=xY6Oxkhd12M "Fine Positioning ")



 

**Project Management**
- Trello board: https://trello.com/b/2IwKx6dv/robotics-engineering-m2

## Authors
Meldrick Reimmer, Selma Boudisssa and Sonizara Danie


## Project Supervisors
Ralph Seulin, Raphael Duverne and Marc Blanchon.
 


