
## Task 1: Sidewalk following

![task1 GIF](media/task1.gif)

Delivery robots need to be able to navigate safely through street sidewalks as they move from pick up to drop off locations. In this task, we have simplified the sidewalk following problem by adding lanes to the sidewalk. Hence, teams are required to develop software to navigate the robot within the lanes from start to end position. Bear in mind that along with lane following, the robot would be required to avoid obstacles which may lie in its path.

**Task 1 Goal:** The goal of this task is to autonomously control the delivery robot from the start position (initial spawned location) to a goal location on the side walk (to be specified).

- To do this, you need to develop software which *processes sensory information* from the robots sensors (camera and LiDAR) and *generates velocity commands* to control the robot's motion [see here for details].


### Task Guidelines

!!! note
    Make sure you have completed the **Getting Started Tutorials** before starting the tasks.

- Run the following launch file to bring up the delivery robot in the world in a new terminal <br>
    ``` 
    roslaunch parc-robot task1.launch
    ``` 
    <br>
- You should see the display below in Gazebo. To the right, there's the robot and to the left is the orange-red sphere which represents the **goal location**.

![task1.1](media/task1.png)

- The two locations (robot initial position and goal location) can be set dynamically by passing arguments in the `roslaunch` command:
    - For updating robot initial position: <br>
    ``` 
    roslaunch parc-robot task1.launch robot_x:-30.43 robot_y:-5.17 robot_yaw:1.57
    ```
    - For updating goal location: <br>
    ``` 
    roslaunch parc-robot task1.launch goal_x:-12.28 goal_y:2.54
    ```

- You need to create a new launch file in your ROS package which runs ALL the code you need in your solution. Name this launch file: `task1_solution.launch`.

So the whole task with solution would wokr by calling both the commands shown below simultaneously,
```
roslaunch parc-robot task1.launch
```
and in another terminal
```
roslaunch <your-package-name> task1_solution.launch
```


- While developing, we recommend you play around with different start and goal positions to ensure your solution is robust.

- The time-limit to complete this task is **5 minutes (300 secs)**.

!!! note
    Ensure you DO NOT provide a solution with hard-coded positions for the robot to move to or hard-coded obstacle positions because in evaluation, the robot initial position, goal location and locations of obstacles (postbox, fire hydrant, etc.) would be randomized.


### Scoring
The score for this task would be determined using the following metrics:

* Out-of-lane distance penalty
* Final distance from goal location (i.e. euclidean distance from goal position at time-limit)
* No. of collisions penalty
* Completion time
