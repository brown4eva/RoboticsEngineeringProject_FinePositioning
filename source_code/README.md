# FINE POSITIONING
**Steps To Follow :**

- Open terminal
   
      $ ssh turtlebot@................(connect to your turtlebot IP)
      $ roslaunch turtlebot_bringup minimal.launch

- Open new terminal
  
      $ ssh turtlebot@.................(connect to your turtlebot IP)
      $ roslaunch freenect_launch freenect.launch publish_tf:=false



**NOTE :**
We created this launch file named fine_positioning.launch which constitutes the ar_large_marker_kinect.launch, the rviz and the script ar_follower.py . 

- Open new terminal

       $ roslaunch fine_positioning fine_positioning.launch 
       
  
  









