# How to set up your workspace


In this tutorial, you will set your set up a directory on your ROS-enabled PC as your workspace for development and install the competition ROS packages. Please follow the instructions below carefully.

!!! note
    This can ONLY be completed after you have set up your PC (by following the previous tutorial)

### Setup ROS workspace

<!-- First, we create a new directory in your home directory called `catkin_ws` with a subdirectory `src`. Then we initialize the directory as a catkin workspace. -->

Open a new terminal on your PC, then copy and paste the following one line at a time:
```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
catkin_init_workspace
```
<br>

### Clone the repository

In the same terminal (or in a new one), copy and paste the following:
```
cd ~/catkin_ws/src
git clone --recurse-submodules https://github.com/PARC-Robotics/parc-robot.git
```
<br>

### Install dependencies

In the same terminal (or in a new one), copy and paste the following:
```
cd ~/catkin_ws
sudo apt update
rosdep install --from-paths ./src --ignore-src -y
```
<br>

### Compile packages
```
cd ~/catkin_ws
catkin_make
source ~/catkin_ws/devel/setup.bash
```

<br>

### Set up ROS environment
To set the environment every time you launch a new terminal, following this command:

```
echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

As you develop, it is good to set the environment variables whenever you run a `catkin_make` command to compile changes to your packages. You can do that by:
```
source ~/catkin_ws/devel/setup.bash
```

<br>

### Test installation

If you completed the preceding tasks successfully, you should be able to run this ROS launch command and see the Gazebo simulator and RViz simulator open with the following display:
```
roslaunch parc-robot robot.launch
```
<br>
