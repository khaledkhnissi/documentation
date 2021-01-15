# How to Submit

Teams would submit their solution of ROS packages as zip.

Below is the expected folder structure of your files.
```
~/catkin_ws/src
├── CMakeLists.txt
├── parc-engineers-league
│   ├── parc-robot
│   │   ├── .
│   │   ├── .
│   │   ├── CMakeLists.txt
│   │   └── package.xml
│   ├── .
│   └── .
└── <YOUR_SOLUTION_FOLDER>        # Zip this folder and submit
    ├── <your_ros_package1>
    │   ├── .
    │   ├── .
    │   ├── CMakeLists.txt
    │   └── package.xml
    ├── <your_ros_package2>
    │   ├── .
    │   ├── .
    │   ├── CMakeLists.txt
    │   └── package.xml
    ├── .
    ├── .
    ├── .
    ├── .
    └── README.md                   # Required
```

A README file (either .txt, .md, or .pdf) with the following information is **MANDATORY** in the zip package:

* List all the packages installed and used in your solution.
* Provide commands required to run your solution. This should be:
    - Task 1: ` roslaunch <your-package-name> task1_solution.launch `
    - Task 2: ` roslaunch <your-package-name> task2_solution.launch `
    - Task 3: ` roslaunch <your-package-name> task3_solution.launch `

 **NOTE:** Please ensure you include all the packages (dependencies) used in your solution in your package's "package.xml" file [see guide](http://wiki.ros.org/rosdep/Tutorials/How%20to%20add%20a%20system%20dependency). <br>

The zipped folder should be uploaded using this *solution submission form*.
