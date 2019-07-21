# navigation
This repository contains the files necessary for Project 1 of the Udacity's Deep RL ND.

## Project Environment and Dependencies
The code is written in Python3 and PyTorch.  Unityagents package has the problem environment, described in the section below.
Dependencies are specified in the requirements file and can be installed by:
```
pip install -r requirements.txt
```

## RL Problem Environment
This project uses Reacher environment, from Unity.

![Alt Text](https://s3.amazonaws.com/video.udacity-data.com/topher/2018/June/5b1ab4b0_banana/banana.gif)

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

0 - move forward.

1 - move backward.

2 - turn left.

3 - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

## Training the Agent
The individual cells in notebook ```Continuous_Control.ipynb``` can be executed sequentially to train the agent. Note that after training, this file saves the Q-Network NN weights in the checkpoint.pth files.  Additionally, note that these files are provided in the git repo and a re-run will cause these files to be generated with the new run.

If you just want to see the performance, the use the ```Saved_Agent.ipynb```. Execute the only cell in the notebook.  The code loads the actor and critic NN weights and runs the environment for 200 time steps before terminating.
