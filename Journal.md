# FYP Development Journal

This journal documents the weekly progress of my Final Year Project (FYP).
Each entry contains the goal for that week, broken down into actionable tasks with their completion status.
Each weekly entry is labeled as `Week N — DD MM YY`, where the date representsthe Sunday that begins that week.

**Project:** Human-Robot collaboration using vision based intent prediction for a shared task in a shared workspace.

**Author:** Zain Ali Zaihid 

**Institution:** UET, Lahore

## Week 1 — 19-04-26

### Goal
Set up the working environment and develop a single Joint Space example for FER that runs on sim and hardware.

### Tasks
- [x] Set up Ubuntu 22.04
- [x] Install ROS2 Humble
- [x] Set up Gazebo
- [x] Install libfranka 0.8.0
- [x] Set up `franka_ros2` drivers
- [ ] Develop a single Joint Space example that runs on sim and hardware

### Discussion
Encountered libfranka compatibility issue. The driver, franka_ros2, uses libfranka v0.9.2 while, the available panda robot was using v0.8.0 (FCI 4.2.0). The issue was resolved by updating the FCI version to 4.2.2. The Driver uses docker with ros2 and mujuco. Moving on development will be done within this docker environment.

## Week 2 — 26-04-26

### Goal
This week, focus will be on understanding the frnaka_ros2 driver and libfranka, inverse kinematics and system communication flow. A simple pick and place example will also be implemented and tested on both, hardware and simulation.

### Tasks
- [ ] Explore `franka_ros2` driver setup and structure  
- [ ] Study `libfranka` API and its usage  
- [ ] explore inverse kinematics (IK) for Panda  
- [ ] Analyze communication flow between ROS2, driver, mujoco and robot hardware  
- [ ] Implement a basic pick-and-place example in simulation and hardware  
