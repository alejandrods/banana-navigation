# banana-navigation
Udacity deep reinforcement learning navigation project

</br>

## Project details
This project uses an Unity environment. The environment is a flat plain with bananas scattered around. There are 2 types of bananas: yellow bananas and blue bananas. The objective is to collect yellow bananas and avoid blue bananas. 

+1 is given as reward for collecting a yellow banana and -1 for collecting blue banana.

There are 4 actions available: 0 - move forward, 1 - move backward, 2 - move left, 3 - move right.

The state space has 37 dimensions.

Environment is considered solved when an average reward of +13 for 100 episodes is reached.

</br>

## Getting started
The project is written using Jupyter Notebook.
This command needs to be run to install the needed packages:

```
!pip -q install ./python
```
Running all the cells in the notebook will install it automatically.

</br>

## Instructions
The project consists of 5 files:
* navigation-project.ipynb - run this file in Jupyter Notebook
* nav_agent.py - the Agent class
* nav_model.py - the DQN models
* checkpoint.pth - saved trained model to use
* Report.md - description of the implementation

Switching between DQN model and Dueling DQN is done at cell 4 by setting dueling to True/False

Switching Prioritized Experience Replay is also done at cell 4 by setting prioritize to True/False
```
agent = Agent(state_size=37, action_size=4, seed=0, dueling=False, prioritize=False)
```


