# av_course_schoolPC
#Task 3: Autonomous Navigation of Ego Vehicle Using Autoware
**Prerequisites**

    ROS 2 (e.g., Foxy, Galactic, Humble)
    Autoware installed and sourced
    Functional planning simulator with sample map
    Docker (optional but recommended for Autoware compatibility)
    A built and sourced workspace

#Setup Instructions
**Clone the repository and build the workspace**

Navigate to your ROS 2 workspace

cd ~/ros2_ws

Clone this repository

git clone https://github.com/Edgar-overclock/av_course_schoolPC

Go back to workspace root

cd ~/ros2_ws

Build all packages

colcon build --symlink-install

source setup.bash

**Run the programm**

ros2 launch my_robot_controller car_nav.launch.py
