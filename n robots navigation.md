# This package is for controlling multiple TB3 on Gazebo and RViz

```
$ cd /catkin_ws/src

$ git clone https://github.com/raghdutionn/N-Robots-Navigation 

$ cd .. (go back to parent directory)

$ catkin_make

$ cd 

$ source ~/catkin_ws/devel/setup.bash

$ sudo apt-get install ros-melodic-turtlebot3

$ sudo apt-get install ros-melodic-turtlebot3-gazebo

$ sudo apt-get install ros-melodic-turtlebot3-navigation

$ roscore (1st tab)

$ export TURTLEBOT3_MODEL=burger (2nd tab)

$ roslaunch turtlebot3_gazebo turtlebot3_world_multi.launch 
```
note: if you got an error like this: 

![VirtualBox_Ubuntu 18 4 Bionic_23_08_2021_06_22_14](https://user-images.githubusercontent.com/53378171/130536835-28599ade-1ad1-49ad-97d3-2d6761efdaf8.png)

just go to the exact directory and launch the file, and hopefully it'll work

![VirtualBox_Ubuntu 18 4 Bionic_23_08_2021_06_34_18](https://user-images.githubusercontent.com/53378171/130537284-60d00189-396f-48ea-8330-ce9fa81e16d3.png)

![VirtualBox_Ubuntu 18 4 Bionic_23_08_2021_06_47_26](https://user-images.githubusercontent.com/53378171/130537180-c4d5e6fd-565a-40f2-a43d-a350b6741cd0.png)


---


```
$ export TURTLEBOT3_MODEL=burger (3rd tab)

$ roslaunch turtlebot3_navigation turtlebot3_navigation_multi.launch
```

![VirtualBox_Ubuntu 18 4 Bionic_23_08_2021_07_30_45](https://user-images.githubusercontent.com/53378171/130537406-84fa6382-2f78-4f91-afe2-4dc7bc74b179.png)




after you adjust each robot's laser to the map using 2D Pose Estimate (notice there are two **2D pose Estimate** and **2D Nav Goal** for *each robot*) you'll see the map like this:

![VirtualBox_Ubuntu 18 4 Bionic_23_08_2021_07_54_18](https://user-images.githubusercontent.com/53378171/130537770-25185083-29a6-458a-bd1a-37a836ea931e.png)



---

```
$ rostopic list (to see the topics)
```
![VirtualBox_Ubuntu 18 4 Bionic_23_08_2021_07_57_00](https://user-images.githubusercontent.com/53378171/130537848-63b7181f-3af8-4721-bd34-7762f4fce8f3.png)


---

```
$ rosrun rqt_graph rqt_graph
```
![rosgraph](https://user-images.githubusercontent.com/53378171/130538265-1d10504b-78ce-4eeb-a87d-a0bceaaa1ab2.png)



### Final Result:
https://user-images.githubusercontent.com/53378171/130535975-1c63edd2-b38d-477b-95d9-1df8b4bbf541.mov



## Resources:

[1] - https://github.com/syahmi001/multinav_turtlebot3/tree/f4ab06f46fb0b8d13386ec61e46b4ff756de0269

[2] - https://github.com/ROBOTIS-GIT/turtlebot3
