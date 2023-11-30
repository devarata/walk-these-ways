# Walk-these-ways (CS562: Advanced Robotics)
[Fall23-Advance_Robotics-Project (3).pdf](https://github.com/devarata/walk-these-ways/files/13515748/Fall23-Advance_Robotics-Project.3.pdf)


## Introduction

This project, part of CS562: Advanced Robotics, is an endeavor to train and demonstrate a robotic dog's ability to navigate and avoid obstacles. It leverages the Isaac Gym Simulator and the Unitree Go1 robot, focusing on achieving precise locomotion and navigation in a virtual environment. The project's ultimate goal is to enable the robot dog to move from point A to point B while avoiding collisions, simulating real-world scenarios where such technology could be vital in search and rescue, agriculture, logistics, and healthcare.

## Phase 1: Robot Locomotion

### Overview
Phase 1 aims to train a velocity-conditioned neural network policy. This policy will enable the robot to walk at commanded longitudinal, lateral, and angular velocities. The sensory data includes joint positions, velocities, and orientation of the gravity vector, which are essential for the robot's stable movement.

### Implementation
The phase begins with setting up the Isaac Gym simulator and then cloning the 'walk-these-ways' repository. The main task is to train the robot to follow commanded velocities within a specified range, familiarizing participants with the simulator, code base, and the robot's functionality.

### Results

[![Thumbnail for Plan] <img width="649" alt="Thumbnail for Plan" src="https://github.com/devarata/walk-these-ways/assets/26374240/ce707891-98ac-499a-8705-3ab2c040decc">](https://github.com/devarata/walk-these-ways/assets/26374240/016eeea5-06d1-4222-a2b2-8b2704595964)


## Phase 2: Robot Navigation within Walls

### Overview
Building on Phase 1, Phase 2 focuses on navigating a walled corridor without colliding. This involves training another policy using reinforcement learning, Actor-Critic Proximal Policy algorithm (PPO), which will provide velocity commands to the locomotion policy. The robot dog can have a fixed as well as random initialization.

### Implementation
The task involves setting up an environment with walls, implementing a Navigator class, and employing the Actor-Critic Proximal Policy algorithm for training. The challenge is to navigate the robot from a start to a goal position, varying the initial position and orientation of the robot.


### Results

#### Dog walking towards the goal line (Fixed spawning)
[![Thumbnail for Plan] <img width="649" alt="Thumbnail for 80" src="https://github.com/devarata/walk-these-ways/assets/26374240/295e7282-7268-401d-b7f6-968c5371475e">](https://github.com/devarata/walk-these-ways/assets/26374240/847c28d1-dace-42f2-8d15-b2940c2dad3d)

#### Dog walking towards the goal line (Backward - Random spawning)
[![Thumbnail for Plan] <img width="649" alt="Thumbnail for 80" src="https://github.com/devarata/walk-these-ways/assets/26374240/295e7282-7268-401d-b7f6-968c5371475e">](https://github.com/devarata/walk-these-ways/assets/26374240/a3112c08-bb4b-4d5a-96c8-add0d4eb1471)

#### Dog realigning itself towards the goal line (Forward - Random spawning)
[![Thumbnail for Plan] <img width="649" alt="Thumbnail for 80" src="https://github.com/devarata/walk-these-ways/assets/26374240/295e7282-7268-401d-b7f6-968c5371475e">](https://github.com/devarata/walk-these-ways/assets/26374240/a95445a4-54fc-4f25-afff-d139e6a6eb21)



## Phase 3: Robot Locomotion with Obstacle Avoidance (In progress)

### Overview
The final phase introduces obstacle avoidance to the navigation policy. The policy now needs to consider the obstacle's location and size in the environment.

### Implementation
We add an immovable obstacle to the existing environment and train the policy to avoid it. The input space should include the obstacle's location and size.


#### Diagram of the environment with the obstacle
<img width="516" alt="Box with Obstacle Environment" src="https://github.com/devarata/walk-these-ways/assets/26374240/28904218-c62a-4a9c-84fa-17b79bf1207d">













