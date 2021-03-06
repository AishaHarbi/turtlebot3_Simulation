# turtlebot3_Simulation
## Turtlebot3 Installation and Simulation: ubuntu 20.04 ROS NEOTIC 
prerequisite: You have to have ROS installed on your system, have a catkin workplace set up already and have created a catkin package inside the your workplace. 
### Turtlebot3 Installation:
#### To install the dependcies, open your terminal and navigate to your workplace folder:

**cd ~/[your workplace folder name]/src/**

#### Install the dependcies: 

**git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git**

**git clone https://github.com/ROBOTIS-GIT/turtlebot3.git**

**cd ~/catkin_ws && catkin_make**

### Now you have to choose a turtlebot3 model (burger, waffle, waffle pi) 
[check this for more info](https://emanual.robotis.com/docs/en/platform/turtlebot3/export_turtlebot3_model/)

#### Type in this command to open the bashrc file to add the turtlebot3 model:

**gedit ~/.bashrc**

Add this line at the bottom of the file:

**export TURTLEBOT3_MODEL=burger**
save the file and close it. 
#### source the bashrc file by running: 
**source ~/.bashrc**

Now to install the simulation files run the following command( to navigate to your workplace folder then the source folder): 

**cd ~/[your workplace name]/src/**

then: 

**git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git**

### Turtlebot3 Simulation:
first navigate to your workplace folder: 
**cd ~/[your workplace name]/src/**

then run the following command to source the bash file:

**source home/[your name]/[your workplace folder name]/devel/setup.bash

### Just as an example I ran the gezebo turtlebot: 
**roslaunch turtlebot3_gazebo turtlebot3_world.launch**

###### Then to control the robot to move around in its little world. Open a new tab and run the following command:

source the bash file:

**source home/[your name]/[your workplace folder name]/devel/setup.bash

then run the following command 

**roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch** 

Now You can freely control the robot's movement via the terminal just like in the following screenshot:

![Screen Shot 2020-07-07 at 20 04 18](https://user-images.githubusercontent.com/45641051/86818235-cae33b80-c08e-11ea-82c1-2304d5a9a27b.png)

