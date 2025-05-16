
# Task 3: Autonomous Navigation of Ego Vehicle Using Autoware

**Prerequisites**

    ROS 2 (e.g., Foxy, Galactic, Humble)
    Autoware installed and sourced
    Functional planning simulator with sample map
    Docker (optional but recommended for Autoware compatibility)
    A built and sourced workspace

# Setup Instructions

**Clone the repository**

Navigate to your ROS 2 workspace

cd ~/ros2_ws

Clone this repository

git clone https://github.com/Edgar-overclock/av_course_schoolPC

**Enter the docker**

xhost +local:docker

docker run -it --rm --privileged --env=DISPLAY --env=QT_X11_NO_MITSHM=1 -v /tmp/.X11-unix:/tmp/.X11-unix -v /home/autolab/ros2_ws:/ros2_ws -v /home/autolab/autoware_map:/autoware_map --workdir /ros2_ws mohsen_aw:full bash

**Build the workspace**

Build all packages

colcon build --symlink-install

source setup.bash

**Run the programm**

ros2 launch my_robot_controller car_nav.launch.py
