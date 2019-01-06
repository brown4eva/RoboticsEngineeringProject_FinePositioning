# Creating the Marker

**Steps To Follow :**

- Installation of ar track alvar package
 
       $ sudo apt-get install ros-indigo-ar-track-alvar*
       

- Downloading rbx2 package from Pirot github

      $ git clone https://github.com/pirobot/rbx2


- Select the right location

      $ roscd rbx2_ar_tags/data
      
- Create your own tag

      $ rosrun ar-track-alvar createMarker0

- Viewing the marker

      $ eog MarkerData_0.png
      
      
 ## Created Marker
 
 <p align="center">
<img src="/source_code/fine_positioning/data/MarkerData_0.png" width="300">
</p>
