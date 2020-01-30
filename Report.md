## Learning Algorithm

As a base i have used Deep Deterministic Policy Gradient (DDPG) from the course: https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum  
Particulary, i have used my working solution for [Project 2 - Continous Control](https://github.com/gkowalik/ContinousControl) and there will be many similarities.
  
As this task uses two agents (or we can use one agent playing both sides) some modifications were needed. I have explored both options - to use one agent playing both sides or two independent agents. Two agent solution had slithly better results for me.  

Other changes to source DDPG (same as in project 2):  

1. I have added epsilon parameter to reduce noise by some multipler (0.997) each episode.  I have also reduced initial sigma to sigma=0.18 
2. Instead of training every episode i have parametrized how often and how many times training happen. 
3. Number of units in neural networks for agents and critics: fc1_units=400, fc2_units=300
4.  I have tuned hyperaparemeters, most significant changes are increase on batch size and reducing gamma 

Final parameters, along with other hyperparameters:  

BUFFER_SIZE = int(1e6)  # replay buffer size
BATCH_SIZE = 120        # minibatch size
GAMMA = 0.99           # discount factor
TAU = 5e-2              # for soft update of target parameters
LR_ACTOR = 1e-4         # learning rate of the actor 
LR_CRITIC = 1e-3        # learning rate of the critic
WEIGHT_DECAY = 0        # L2 weight decay
EPSILON_DEC =0.9997   #noise reduction
TRAIN_FREQ=5     #how often train agent
TRAIN_N=2      #how many times train agent

5. I have added workspace "keep alive" solution I have also added  [provided solution](https://github.com/udacity/workspaces-student-support/tree/master/jupyter) to keep workplace active as [suggested in QA](https://knowledge.udacity.com/questions/61260). It requires workspace_utils.py file provided in this repository.

## Plot of Rewards
![Plot](https://raw.githubusercontent.com/gkowalik/Collaboration_and_Competition/master/plot.png "Plot")
Plot shows average of max score (average maximum from 2 agents for each episode), therefore averages for each agents can be little lower.
Environment was solved in 832 episode and ended on 932  episode (having average from 832-932  episode above required 0.5)

More details and results per episode are avaliable in [Main project file](https://github.com/gkowalik/Collaboration_and_Competition/blob/master/Tennis.ipynb)


## Ideas for future work

to do
