# Temporal Memory-based RRT (TM-RRT) Exploration Simulation (ROS Melodic)
This directory showcases the simulation stage for the TM-RRT Exploration using Gazebo and RVIZ.

## Requirements
The following code is executed in ROS Melodic in Ubuntu 18.04 LTS, Python 2.7

The following libraries are required to be installed before proceeding to run the code

    $ sudo apt-get install ros-melodic-gmapping
    $ sudo apt-get install ros-melodic-navigation
    $ sudo apt-get install python-opencv
    $ sudo apt-get install python-numpy
    $ sudo apt-get install python-scikits-learn
    $ sudo apt-get install ros-melodic-teb-local-planner
    $ sudo apt-get install ros-melodic-multirobot-map-merge

    
## Installation Process
Create a new folder called "catkin_explore/src" by executing the following comment:

    $ sudo mkdir -p ~/catkin_explore/src
    $ cd ~/catkin_explore/src/
    $ git clone -b main-Melodic https://github.com/hikashi/TM-RRT_exploration_Simulation.git
    $ cd ~/catkin_explore
    $ catkin_make
    
## Instruction for Running Simulation
In console one (for running small map):
    
     $ roslaunch ros_3d_multitb3 multiple_tb3_house4.launch
In console one (for running big map):
    
     $ roslaunch ros_3d_multitb3 multiple_tb3_house5.launch

In console two:
 
     $ roslaunch tmrrt_exploration trio_exploration.launch
     
     
     
 
## Setting up Simulation for testing
An example of the simulation can be shown in the following video: 

[![TM-RRT Exploration for Ubuntu 18.04 ROS Melodic](https://img.youtube.com/vi/F40GGvnIfsc/0.jpg)](https://www.youtube.com/watch?v=F40GGvnIfsc "TM-RRT Exploration for Ubuntu 18.04 ROS Melodic")
