# Creation of Map
**Steps To Follow :**
- Open terminal

      $ ssh turtlebot@...........(connect to your turtlebot IP)
      $ roslaunch turtlebot_bringup minimal.launch

- Open New terminal
             
      $ ssh turtlebot@............(connect to your turtlebot IP)
      $ roslaunch turtlebot_navigation gmapping_demo.launch

- Open New terminal
       
      $ roslaunch turtlebot_rviz_launchers view_navigation.launch
      
  
- Open New terminal
       
       $ jstest /dev/input/js0
       $ ctrl c
       $ roslaunch turtlebot_teleop logitech.launch --screen
       
**Make sure you start the recording before navigating the robot with the teleop**  

  
## RECORDING THE MAP

- Open terminal
     
      $ roscd rbx1_nav/bag_files(choose your own path)
      $ rosbag record  my_scan_data/scan/tf
      $ roscd rbx1_nav/map
      $ rosrun map_server map_saver -f roboticroom_map (choose the name of your map) 
      
     
     
## Related Video & Map Saved

[![](http://img.youtube.com/vi/GcMuJutT3g0/0.jpg)](http://www.youtube.com/watch?v=GcMuJutT3g0 "Navigating using Teleop")  <img src="/Materials/images/map.JPG" width="300"> 

      
      




















      



