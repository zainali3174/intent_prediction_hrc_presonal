# Human Intent Prediction for Proactive Human-Robot Collaboration

## Overview

This project focuses on enabling safe, intelligent and proactive human-robot collaboration using a robotic manipulator. The system is designed to operate in a shared workspace where a robot and a human collaboratively perform a structured task—stacking randomly placed cubes in a predefined sequence.

The robot adapts to human actions in real time, corrects errors, and predicts human intent to improve efficiency and safety.

---

## Objectives

* Develop a system for real-time human detection and tracking
* Detect and localize cubes within the workspace
* Implement task-level planning for collaborative stacking
* Enable robot response to human actions (correct/wrong placement)
* Predict human intent based on motion and interaction patterns
* Ensure safe operation through collision avoidance and workspace monitoring

---

## Hardware and Technologies Used

* Franak Emika Panda, aka FER (FCI v4.2.2)
* Intel RealSense RGB-D camera
* OS (Ubuntu 22.04)
* ROS 2 (Humble)
* Mujoco 
* Frnak_ros2 Driver
* MoveIt 
* YOLOv11 
* Python / C++

---

## Use Case: Collaborative Cube Stacking

The robot and human work together to stack cubes in a predefined order.

### System Behavior

* If the human places the correct cube → robot proceeds to next task
* If the human places the wrong cube → robot removes and replaces it
* If the human reaches for a cube → robot pauses and predicts intent
* If the human changes intention → robot replans accordingly

---

## Safety Features

* Continuous human detection in workspace
* Collision avoidance mechanisms
* Collision detection using built-in sensors
* Safe stopping or trajectory adjustment when human is nearby

---
This is a personal repo maintained by @zainali3174. Team repo available at https://github.com/zainali3174/vision_intent_prediction_hrc.git
---

## Notes

This project is part of a Final Year Project (FYP) focused on combining robotics, computer vision, and machine learning to enable intelligent human-robot interaction.

