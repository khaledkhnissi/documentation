# Phase 1: Simulation

In this simulation-only phase, teams would work on providing solutions to three (3) fundamental tasks of a delivery robot which are: 

* Sidewalk following (with obstacle avoidance)
* Traffic sign detection and recognition
* Go-to-goal navigation (with obstacle avoidance)

The simulation platform to be used in this phase is the [Gazebo Simulator](http://gazebosim.org/). Teams are required to develop, test and submit software to successfully complete these tasks autonomously. This phase will evaluate the teams' capabilities to successfully complete these fundamental tasks required to compete in phase 2 (on the physical robot).

Teams are provided with the delivery robot ROS packages and Gazebo environment models to enable them develop and test their solutions (see [GitHub Repository](https://github.com/PARC-Robotics/PARC-Engineers-League)).

Each task is designed as stand-alone, not depending on other task functionalities, hence, we request teams to complete the tasks separately. The tasks would be evaluated individually and the total team score for this phase would be the sum of individual task scores.


_____________________________________________________________________________

<br>

_____________________________________________________________________________

<br>

_____________________________________________________________________________

<br>

## What to Submit
Teams would submit a zipped folder containing the following:

* Complete catkin workspace **src folder** containing all the installed packages used to complete the task.
* A README file (either .txt, .md, or .pdf) with the following information:
    * List all the packages installed and used in your solution.
    * Provide commands required to run your solution. This should be: <br>
    Task 1: ` roslaunch <your-package-name> task1_solution.launch ` <br>
    Task 2: ` roslaunch <your-package-name> task2_solution.launch ` <br>
    Task 3: ` roslaunch <your-package-name> task3_solution.launch `
* **NOTE:** Please ensure you include all the packages (dependencies) used in your solution in your package's "package.xml" file [see guide]. <br>

The zipped folder should be uploaded using this *solution submission form*.
