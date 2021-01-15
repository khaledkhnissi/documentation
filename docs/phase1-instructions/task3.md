
## Task 3: Go-to-goal navigation

![task3 GIF](media/task3.gif)

### Task Guidelines
- **Goal:** Implement software which processes sensory information from the robots sensors (camera and LiDAR) and generates velocity commands to control the robot's motion to move from the start position towards to drop off which is in front of the person standing in the park.
- **Step 1:** Review the "Task 3" folder in the Github repository.
- **Step 2:** Complete the [Setting up your PC] and [Setting up workspace] steps (if you have not already done so).
- **Step 3:** Run the following launch file to bring up the robot in the designated world in a new terminal <br>
` roslaunch <our-robot-package-name> task3.launch `


You should see the display below in Gazebo. There is a orange-red sphere which represents the **goal location**.

![task1.1](media/task3.png)

### Scoring
The score for this task would be determined using the following metrics:

* No. of collisions penalty
* Final distance from goal (set time limit)
* Completion time
