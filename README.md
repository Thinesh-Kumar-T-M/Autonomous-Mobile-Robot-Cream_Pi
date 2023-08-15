# Autonomous-Mobile-Robot-Cream_Pi
![Screenshot from 2023-08-15 15-55-03](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/c4873930-dc25-4f2b-9369-cad738c7e899)![Screenshot from 2023-05-18 17-11-31](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/263dbd75-a2d3-4d63-9f06-71f3e3cd0f43)

## Hello all ! 👋<br>
>Looks cool right !! Let's get it working in your device too comon ....<br>
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
You should have these 3 packages in your *src* folder.
![cream_pi_packages](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/d3120b00-9008-4db0-a8de-e073056aa680)


### Step 2:
Deploy the AMR with a pre-built environment (in this case a _house environment in Gazebo_) by launching the **cream_pi_house.launch**
```
roslaunch cream_pi_gazebo cream_pi_house.launch
```
![Screenshot from 2023-05-18 17-08-35](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/8452464d-f269-40a5-ac20-aa864814f121)

### Step 3:
Visualise in  RViz by launching another file called **display.launch**<br>
_Open a new terminal_
```
roslaunch cream_pi display.launch
```
![Screenshot from 2023-05-18 17-08-45](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/3076e3b2-53aa-4491-bfd8-0e69d41e27f0)

### Step 4:
Start the Autonomous Navigation<br>
_In another terminal_
```
roslaunch cream_pi_navigation cream_pi_navigation.launch
```
### Step 5:
Go to the opened RViz window and Specify the _Final Position_ of the robot to which it has to go by:<br>
>1. Click _2D Nav Goal_ from the RViz Menu bar.
![2dnavgoal](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/29ebf09e-fdb3-4f0e-861e-647ef2db13b9)

>2. Using the mouse click and hold the point to which you want the robot to navigate.(_Point must be within the map_)![Screenshot from 2023-08-15 17-54-42](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/18fe20dc-3a06-44b1-a109-80b73f5aada1)

>3. Point the arrow in the direction you want the robot to pose finally.![Screenshot from 2023-08-15 17-54-47](https://github.com/Thinesh-Kumar-T-M/Autonomous-Mobile-Robot-Cream_Pi/assets/82699150/74387a08-243f-42f0-84b0-3a25117848b1)


## You can see the robot navigating to the desired position both in Gazebo and RViz simultaneously.
