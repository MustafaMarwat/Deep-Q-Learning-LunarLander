# Deep Q-Learning Lunar Lander

In this repository, I present a Reinforcement Learning (RL) project where I train an agent to land a lunar lander safely on a landing pad on the surface of the moon. The goal of the project is to implement a Deep Q-Learning algorithm with Experience Replay to teach the agent how to navigate and land the lunar lander effectively.


## Table of Contents

- [Project Description](#project-description)
- [Environment](#environment)
- [Project Structure](#project-structure)
- [Hyperparameters](#hyperparameters)
- [Training the Agent](#training-the-agent)
- [Results](#results)
- [References](#references)
- 
## Project Description

In this project, I utilized the OpenAI Gym toolkit to access the Lunar Lander environment. The agent's objective is to safely land the lunar lander on the landing pad, and the environment offers discrete actions and state observations, making it suitable for reinforcement learning.

The main components of the project include:

1. Importing necessary packages.
2. Defining hyperparameters for the learning process.
3. Setting up the Lunar Lander environment.
4. Implementing Deep Q-Learning with Experience Replay.
5. Training the agent to learn optimal landing strategies.
6. Visualizing the results.

## Environment

The Lunar Lander environment is provided by OpenAI's Gym toolkit. The agent has four discrete actions available:

1. Do nothing.
2. Fire right engine.
3. Fire main engine.
4. Fire left engine.

The agent's state observation includes its coordinates, linear velocities, angle, angular velocity, and two booleans representing leg contact with the ground. The agent receives rewards based on its actions, such as positive rewards for landing on the pad and penalties for crashing or using the engine. Episodes terminate when the lander crashes or goes out of bounds.



## Project Structure
The project is organized as follows:
- `reinforcement_learning.ipynb`: The Jupyter Notebook containing the complete code for training the lunar lander agent.
- `utils.py`: A Python module containing utility functions used in the project.
- `videos/`: A directory to store videos of the trained agent in action.

## Hyperparameters
The key hyperparameters used in this project are:

- MEMORY_SIZE: Size of the memory buffer for experience replay.
- GAMMA: Discount factor for future rewards.
- ALPHA: Learning rate for updating the Q-network.
- NUM_STEPS_FOR_UPDATE: Number of time steps before performing a learning update.


## Training the Agent
To train the agent, run the provided Jupyter Notebook or Python script. The training process will involve episodes where the agent learns to land the lunar lander safely. The Q-network is updated based on experience replay and target networks to improve the agent's performance.

## Results
The results of the training can be observed by running the provided code. The agent's performance is evaluated based on the total points it accumulates during episodes. The goal is to achieve an average of 200 points in the last 100 episodes, indicating that the agent has successfully learned to land the lunar lander.

## References
To learn more about the concepts and techniques used in this project, you can refer to the following papers and resources:

- Human-level Control Through Deep Reinforcement Learning
- Continuous Control with Deep Reinforcement Learning
- Playing Atari with Deep Reinforcement Learning

Feel free to explore and modify the project to further enhance your understanding of reinforcement learning and its applications.
