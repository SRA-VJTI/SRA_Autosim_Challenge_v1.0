## Theme:
The world continues to move deliberately towards a transportation system driven by autonomous vehicles having benefits like lesser travel time, cheaper transportation costs, reduced CO2 emissions, and many more. But with great power comes great responsibility. Designing a safer mechanism while maintaining an efficient program has always been a top priority. 
A line following vehicle is in a way an entry level autonomous vehicle that can navigate any course while following on a contrasting background. As a line follower bot always needs a path to run, its applications are limited. This is where various sensors like lidar, ultrasonic, camera come into picture. 

## For Problem Statement and Images:
https://drive.google.com/file/d/1-HUtt-bm3C8wKsXfCvsx6lSd64l9kTW4/view?usp=sharing

## STEPS TO FOLLOW:

Clone this repository <br>

Add marker10 and sampleQR to models in .gazebo <br>

Make the following changes in world and launch files in arena_with_qr package <br>

## Sample Arena

Change path in line `7` of `sample_arena.launch`  
   
   ```
        <arg name="world" default="/home/neha_kurian/catkin_ws/src/arena_with_qr/world/sample_arena.world" />
   ```

Change path in line `105` and `127` in `sample_arena.world`

   ```
	<uri>/home/neha_kurian/catkin_ws/src/sample_arena_urdf/meshes/arena_samplenew.dae</uri>
   ```

## Final Arena

Change path in line `7` of `final_arena.launch `
   
   ```
       <arg name="world" default="/home/neha_kurian/catkin_ws/src/arena_with_qr/world/final_arena.world" />
   ```

Change path in line `293` and `315` in `final_arena.world`

   ```
	<uri>/home/neha_kurian/catkin_ws/src/final_arena_urdf/meshes/final_arena.dae</uri>
   ```

## Open terminal from your workspace and do
   
   ```
   catkin_make
   source devel/setup.bash
   ```
   
   Launch sample arena:<br>
   ```  
   roslaunch arena_with_qr sample_arena.launch
   ```
   
   Launch final arena:<br>
   ```
   roslaunch arena_with_qr final_arena.launch
   ```
