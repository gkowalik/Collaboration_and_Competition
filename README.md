# ContinousControl
## My solution for Udacity course "Deep Reinforced Learning"

This is a solution for Project 2 in Udacity course "Deep Reinforced Learning". It is using materials from course, particulary it is based on DDPG solution from course:
https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum

### The Environment

This project is for  [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

### Solving the Environment

I have selected option 1 (from two avaliable) to solve:

Option 1: Solve the First Version
The task is episodic, and in order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes.


### Getting Started

This solution is designed and tested in Workspace evrinoment provided by Udacity. To run it there simply upload all files to Udacity workplace for this project.  

As provided by Course, you can setup your own evrinoment:
#### STEP1:
https://github.com/udacity/deep-reinforcement-learning#dependencies

#### STEP2: 
Download:  

Linux: [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)  
Mac OSX: [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)  
Windows (32-bit): [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)  
Windows (64-bit): [DOWNLOAD](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)  

Then, place the file in the p2_continuous-control/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

<strong><em> NOTE: THIS CODE WAS NOT TESTED OUTSIDE UDACITY WORKSPACE. PARTICULARY, THERE IS A SOLUTION TO KEEP UDACITY WORKSPACE ALIVE (workspace_utils.py) THAT MIGHT NEED TO BE REMOVED</em></strong>

### Instructions

After copying all files to workplace simply run Continuous_Control.ipynb file to train the agent. Solution already provide training results that solved the task.  

Trained agents are stored in checkpoint_actor.pth and checkpoint_critic.pth files.

