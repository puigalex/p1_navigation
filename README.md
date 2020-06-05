# Project 1: Udacity Deep Reinforcement Learning Navigation

### Introduction

This project consists in training an agent to navigate in a 3D environment created in Unity.

The environment consists of a square room filled with several blue and yellow bananas, the agent must be able to learn to navigate through the room avoiding the blue bananas and taking the yellow ones.

### Environment specs

The environment consists of a state space of 37 variables and an action space of 4 (0-Forward, 1-Backward, 2-Left, 3-Right).

Yellow bananas will give the agent a reward of +1 for each banana, while the blue bananas will penalize the agent with a reward of -1.

The goal is to train an agent that is able to have an average score of +13 over 100 consecutive episodes.

### Requirements
To run this project you must install the dependencies in the requirements.txt file as well as installing the Unity environment from one of the following sources:




- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file you donwloaded into the main folder of this project.

### Files

There are 4 main files in this project, each one needed to train, run and save the agent.
* **dqn_agent.py** File containing the Agent class, this class is the one in charge of creating the agent, selecting actions to take given a state, backpropagate learning through the NN model.
* **model.py** File containing the scructure of the neural network from which the agent will learn. You can change the structure in this file to whatever you want (respecting the input of 37 and output of 4) and the **dq_agent.py** will use that structure for the agent.
* **Navigation.ipynb** Jupyter notebook used to initialize the learning unity envornment, the agent class and train the agent through the specified number of episodes.