# Implementation description

</br>

## Learning Algorithm

DQN, Double DQN, Dueling DQN, Prioritized Experience Replay are used for this project.

DQN model is built with Linear layers and Relu activation functions. 4 Layers of size 256 each proved to perform the best.

Dueling DQN model is built with 4 Layers of size 256 each for Features, and 2 layers of size 128 for Advantage and for Value.

Hyperparameters:
* Replay buffer size = 100000
* Batch size = 256
* GAMMA (discount factor) = 0.999
* TAU (for soft update of target parameters) = 0.001
* Learning rate = 0.0005
* Update network evey 16 step

</br>

## Plot of Rewards
Plot of rewards can beseen after the environment is solved.
