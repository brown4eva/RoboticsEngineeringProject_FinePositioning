# NAVIGATION

**Steps To Follow :**

- Open terminal
      
      $ ssh turtlebot@................... (connect to your turtlebot IP)
      $ roslaunch turtlebot_bringup minimal.launch


- Open new terminal

      $ ssh turtlebot@................... (connect to your turtlebot IP)


- Launch your map with the right path...
 
      $ roslaunch turtlebot_navigation amcl_demo.launch map_file:=/home/turtlebot/ros/indigo/catkin_ws/src/fine_positioning/maps/roboticroom_map.yaml

- Open new terminal to visualize the map on Rviz

      $ roslaunch turtlebot_rviz_launchers view_navigation.launch
      
- Open new terminal to launch the node to enable the robot to navigate to a specific location
  
      $ cd ~/catkin_ws/src/fine_positioning/nodes
      $ python go_to_specific_point_on_map.py 
      
      
 ## Related Video
 [![](http://img.youtube.com/vi/YPPbcnevZK8/0.jpg)](http://www.youtube.com/watch?v=YPPbcnevZK8 "Navigating to specific Location With Rviz ")





