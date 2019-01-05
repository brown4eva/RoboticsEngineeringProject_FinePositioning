# Creation of the package

**Steps to follow :**


- Open terminal

       $ cd ~/catkin_ws/src
       
- Choosing the name of the package and dependencies
  
       $ catkin_create_pkg fine_positioning roscpp rospy urdf
       $ cd fine_positioning 
       
  
- Create the directory inside the package

      $ mkdir maps
      $ mkdir nodes
      $ mkdir rviz
      $ mkdir data
      $ mkdir launch 
      $ cd ~/catkin_ws
      $ catkin_make
      $ rospack profile
      






 
       
       
