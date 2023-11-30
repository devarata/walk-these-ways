# Walk-these-ways (CS562: Advanced Robotics)
[Project Document](https://github.com/devarata/walk-these-ways/blob/master/readme/Fall23-Advance_Robotics-Project%20(3).pdf)

## Introduction

This project, part of CS562: Advanced Robotics, is an endeavor to train and demonstrate a robotic dog's ability to navigate and avoid obstacles. It leverages the Isaac Gym Simulator and the Unitree Go1 robot, focusing on achieving precise locomotion and navigation in a virtual environment. The project's ultimate goal is to enable the robot dog to move from point A to point B while avoiding collisions, simulating real-world scenarios where such technology could be vital in search and rescue, agriculture, logistics, and healthcare.

## Phase 1: Robot Locomotion

### Overview
Phase 1 aims to train a velocity-conditioned neural network policy. This policy will enable the robot to walk at commanded longitudinal, lateral, and angular velocities. The sensory data includes joint positions, velocities, and orientation of the gravity vector, which are essential for the robot's stable movement.

### Implementation
The phase begins with setting up the Isaac Gym simulator and then cloning the 'walk-these-ways' repository. The main task is to train the robot to follow commanded velocities within a specified range, familiarizing participants with the simulator, code base, and the robot's functionality.

### Results
[![Thumbnail for Plan](https://github.com/devarata/walk-these-ways/blob/master/readme/Thumbnail%20for%20Plan.png)](https://github.com/devarata/walk-these-ways/blob/master/readme/plan.mp4)





