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

### What to Submit


## Task 2: Traffic sign detection and recognition


## Task 3: Go-to-goal navigation

