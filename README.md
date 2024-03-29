# State-Estimation-Autonomous-Vehicle

State Estimation for Autonomous Car

## Overview

This repository focuses on the state estimation module for autonomous vehicles, integrating the SBG Systems Inertial Measurement Unit (IMU) for precise and reliable state estimation. The module incorporates the SBG ROS2 Driver to interface with the SBG IMU seamlessly.

## Installation
### Installation from Packages
User can install the sbg_ros2_driver through the standard ROS installation system.
* Galactic ```sudo apt-get install ros-galactic-sbg-driver```
* Foxy ```sudo apt-get install ros-foxy-sbg-driver```

## Requirements

The code has been tested on the following setup:

- **Hardware**: SBG Systems IMU
- **Operating System**: Ubuntu 20.04 (May also work on 22.04)
- **ROS Version**: ROS2 Galactic (Possibly compatible with Humble and Foxy, although not yet tested)
- **Dependencies**: 
  - Robot Operating System (ROS)
  - SBG Driver

## Usage
To run the default Ros2 node with the default configuration

```
ros2 launch sbg_driver sbg_device_launch.py
```

To run the magnetic calibration node

```
ros2 launch sbg_driver sbg_device_mag_calibration_launch.py
```

## Getting Started

Ensure that you have all the requirements satisfied before proceeding.

### Clone the Repository

`git clone https://github.com/HammadSiddiqui30/State-Estimation-Autonomous-Vehicle.git


##  Build
Navigate to the cloned repository directory and build using Colcon:


`cd <repository_directory>`

`colcon build`


If all steps have been successful up to this point, proceed with the following:


Connect the SBG IMU

Run the ekf node in State Estimation.

 `ros2 run state_estimation ekf`




###  Contributions
Contributions to enhance the functionality, efficiency, or compatibility of this perception module are welcome. Please refer to the contribution guidelines for more information.

###  License
This project is licensed under the MIT License. Feel free to use and modify the code.

### TESTING VIDEOS:

[![Watch the video](https://img.youtube.com/vi/yEEOZ6u07oc/0.jpg)](https://youtube.com/shorts/yEEOZ6u07oc?feature=share)

[![Watch the video](https://img.youtube.com/vi/LqnwOVJf_oQ/0.jpg)](https://youtube.com/shorts/LqnwOVJf_oQ?feature=share)



