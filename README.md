# Autonomous-Mobile-Robot-Cream_Pi
### Hello all ! 👋<br>
>With this repository you will be able to deploy and run your own AMR.
Let's get started...🏃‍♂️
<!-- ![BumbyWoolGIF](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/a8720f08-b575-401d-9b43-251118bce398) -->

## Prerequisites:
<ul>
  <li>Ubuntu 20.04 Operating System</li>
  <li>ROS1 </li>
  <li>Gazebo </li>
</ul>

## Simulation of a fully autonomous mobile robot using Gazebo, ROS and RViz. </h2>
### Step 1:
Clone the repository into your ROS workspace.
```
cd ~/caktin_ws/src
git clone https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi
```
Now build your workspace :
```
cd ..
catkin_make
```
### Step 2:
Deploy the AMR with a pre-built environment (in this case a _house environment in Gazebo_) by launching the **cream_pi_house.launch**
```
roslaunch cream_pi_gazebo cream_pi_house.launch
```

### Step 3:
Visualise in  RViz by launching another file called **display.launch**<br>
_Open a new terminal_
```
roslaunch cream_pi display.launch
```

### Step 4:
Start the Autonomous Navigation<br>
_In another terminal_
```
roslaunch cream_pi_navigation cream_pi_navigation.launch
```
### Step 5:
Go to the opened RViz window and Specify the _Final Position_ of the robot to which it has to go by:<br>
>1. Click _2D Nav Goal_ from the RViz Menu bar.
>2. Using the mouse click and hold the point to which you want the robot to navigate.(_Point must be within the map_)
>3. Point the arrow in the direction you want the robot to pose finally.

## You can see the robot navigating to the desired position both in Gazebo and RViz simultaneously.
