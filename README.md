# Collaboration and Competition - Tennis
## My solution for Udacity course "Deep Reinforced Learning"

This is a solution for Project 3 in Udacity course "Deep Reinforced Learning". It is using materials from course, particulary it is based on DDPG solution from course:
https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum

As a core, i have used my working solution for [Project 2 - Continous Control](https://github.com/gkowalik/ContinousControl) and there will be many similarities.

### The Environment

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
- This yields a single score for each episode.

### Solving the Environment

The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.


### Getting Started

This solution is designed and tested in Workspace evrinoment provided by Udacity. To run it there simply upload all files to Udacity workplace for this project.  

As provided by Course, you can setup your own evrinoment:
#### STEP1:
https://github.com/udacity/deep-reinforcement-learning#dependencies

#### STEP2: 
Download:  

Linux: [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)  
Mac OSX: [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)  
Windows (32-bit): [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)  
Windows (64-bit): [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)  

Then, place the file in the p3_collab-compet/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

<strong><em> NOTE: THIS CODE WAS NOT TESTED OUTSIDE UDACITY WORKSPACE. PARTICULARY, THERE IS A SOLUTION TO KEEP UDACITY WORKSPACE ALIVE (workspace_utils.py) THAT MIGHT NEED TO BE REMOVED</em></strong>

### Instructions

After copying all files to workplace simply run [Tennis.ipynb](https://github.com/gkowalik/Collaboration_and_Competition/blob/master/Tennis.ipynb) file to train the agent. Solution already provide training results that solved the task.  

Trained agents are stored in checkpoint_actor1.pth, checkpoint_actor2.pth, checkpoint_critic1.pth  and checkpoint_critic2.pth files.

