
# Offline Development and Troubleshooting


In the last section, we briefly introduced the use of `rosbags` for recording your test runs for later evaluation and troubleshooting. This is a very crucial step, hence, as a starter, we have prepared sample rosbags for you to explore.

<!-- ## Task Guidelines

!!! note
    Make sure you have completed the [**Getting Started in Simulation**](./getting-started-simulation.md) before starting the task. -->

##### 1. Download the ROS bags

- Use this [Google Drive link](https://drive.google.com/drive/folders/1yCpXl-du6hmg1FC_O8ssPQfoHhA02sQn?usp=sharing) to download the ROS bags. 
    - NOTE: The files are large with a total size of ~370MB.

- Save the file on your computer and take note of the directory (it doesn't matter where you store it). For this tutorial, we will use `<rosbag-location>`.


##### 2. Run the ROS bags

- First, open a new terminal and start up `roscore`:

``` shell
roscore
``` 
- In another terminal, open up `rviz`

``` bash
rosrun rviz rviz -d $(rospack find turtlebot3_parc)/rviz/turtlebot3_parc.rviz
```
- Finally, in another terminal, run the `rosbag play` command and pass the ros bag you want to play:

``` bash
# navigate to the <rosbag-location> directory and then run the command:
rosbag play task-part1.bag
```

![task overview](media/rosbag-rviz.gif)

We strongly recommend that you play around with the three rosbags and observe the data carefully to explore best ways to complete the task.

##### 3. Create your own ROS bags

The last task is for you to create rosbags of your own from your team test sessions. For this, start by checking out the [link](http://wiki.ros.org/rosbag/Commandline) for the official documentation on rosbags.

As state in the previous section, give it a try follow the instructions below:
```sh
# in a new terminal on the host PC, run:
rosbag record -a # this is to record all the topics. This might lead to a very large *.bag file

# check out other rosbag commands such as "play", "compress", etc.
```
Follow this [link](https://www.youtube.com/watch?v=Vlp0e89TXpI) for a video tutorial.