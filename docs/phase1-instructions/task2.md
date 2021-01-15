
## Task 2: Traffic sign detection and recognition

![task2 GIF](media/task2.gif)

Road crossing is inevitable for delivery robots as they navigate our streets to complete their delivery task. The task of road crossing is tricky even for humans to complete safely. A major component of the task is monitoring the traffic sign to ensure you comply with it. In this task, you are required to perform traffic sign detection and recognition. We have included a traffic sign with two states (RED and GREEN). 

Teams are required to develop software to use the on-board camera to detect and recognise the state of the traffic sign. 

**Task 2 Goal:** The goal of this task is to perform safe road crossing by detecting and recognising the state of the traffic sign and crossing only when the state is GREEN (GO).


### Task Guidelines

!!! note
    Make sure you have completed the **Getting Started Tutorials** before starting the tasks.

- Run the following launch file to bring up the delivery robot in the world in a new terminal <br>
    ``` 
    roslaunch parc-robot task2.launch
    ``` 
    <br>
- You should see the display below in Gazebo. The traffic sign is initially set to RED and would change to GREEN after the `start_delay` duration is complete.

- While developing, we recommend you play around with different values for the `start_delay` duration by passing an argument as follows:
    
    ``` 
    roslaunch parc-robot task2.launch start_delay:=20
    ```
    <br>

- The time duration from GREEN to RED is set to **20 secs**. This means that you have ~20 secs to cross the road and reach the goal (x=-2.3, y=11.1) after the traffic sign goes green. If the robot is still on the cross walk (i.e. its X position is less than -2.1), the crossing would be considered as failed.

![task2.1](media/task2.png)

!!! note
    Ensure you DO NOT provide a solution with hard-coded move commands for the robot based on a particular `start_delay` value because in evaluation, the `start_delay` value would be randomized. Also, NO hacks for monitoring the state of the traffic sign (such as checking any ROS topics) would be allowed. If it is found out, you will receive a ZERO score for this task.


### Scoring
The score for this task would be determined using the following metrics:

* Reaction time
* Goal completion i.e. has the robot reached the other side of road by the termination of green signal?
* Wrong crossing (binary)
* Completion time
