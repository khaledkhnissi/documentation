# Phase 1: Simulation

In this phase, teams would interact with the delivery robot in simulation (using the Gazebo Robot Simulator). Participants are required to write software to complete three crucial tasks for the operation of a delivery robot:
- Sidewalk following (with obstacle avoidance)
- Traffic sign detection and recognition
- Go-to-goal navigation (with obstacle avoidance)

## Task 1: Sidewalk following
[Image]

Delivery robots need to be able to navigate safely through sidewalks as the move from pick up to drop off locations. In this task, we have simplified the sidewalk following problem by adding lanes to the sidewalk. Hence, teams are required to develop software to navigate the robot within the lanes from start to end position. Bear in mind that along with lane following, the robot would be required to avoid obstacles which may lie in its path.

### Task Guidelines
- **Goal:** Implement software which processes sensory information from the robots sensors (camera and LiDAR) and generates velocity commands to control the robot's motion [see here for details].
- **Step 1:** Review the "Task 1" folder in the Github repository.
- **Step 2:** Complete the [Setting up your PC] and [Setting up workspace] steps.
- **Step 3:** Run the following launch file to bring up the robot in the designated world in a new terminal <br>
` roslaunch <our-robot-package-name> task1.launch `


### Scoring
The score for this task would be determined using the following metrics:
* Out-of-lane distance penalty
* Final distance from goal (set time limit)
* No. of collisions penalty
* Completion time



## Task 2: Traffic sign detection and recognition

### Task Guidelines
- **Goal:** Implement software which uses camera feeds to detect and recognise the state of the traffic sign and control the robot to safely cross the road. Safe crossing means that the robot launches into the road only when the traffic sign is "green" and the robot reaches the other side before it turns "red".
- **Step 1:** Review the "Task 2" folder in the Github repository.
- **Step 2:** Complete the [Setting up your PC] and [Setting up workspace] steps (if you have not already done so).
- **Step 3:** Run the following launch file to bring up the robot in the designated world in a new terminal <br>
` roslaunch <our-robot-package-name> task2.launch `


### Scoring
The score for this task would be determined using the following metrics:
* Reaction time
* Goal completion i.e. has the robot reached the other side of road by the termination of green signal?
* Wrong crossing (binary)
* Completion time




## Task 3: Go-to-goal navigation

### Task Guidelines
- **Goal:** Implement software which processes sensory information from the robots sensors (camera and LiDAR) and generates velocity commands to control the robot's motion to move from the start position towards to drop off which is in front of the person standing in the park.
- **Step 1:** Review the "Task 3" folder in the Github repository.
- **Step 2:** Complete the [Setting up your PC] and [Setting up workspace] steps (if you have not already done so).
- **Step 3:** Run the following launch file to bring up the robot in the designated world in a new terminal <br>
` roslaunch <our-robot-package-name> task3.launch `

### Scoring
* Data to collect: rosbag of TFs
* No. of collisions penalty
* Final distance from goal (set time limit)
* Completion time

## What to Submit
Teams would submit a zipped folder containing the following:
* Complete catkin workspace **src folder** containing all the installed packages used to complete the task.
* A README file (either .txt, .md, or .pdf) with the following information:
    * List all the packages installed and used in your solution.
    * Provide commands required to run your solution. This should be: <br>
    ` roslaunch <your-package-name> task2_solution.launch `
* **NOTE:** Please ensure you include all the packages (dependencies) used in your solution in your package's "package.xml" file [see guide]. <br>

The zipped folder should be uploaded using this *solution submission form*.
