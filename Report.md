# Implementation description

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

## Plot of Rewards
Plot of rewards can be seen after the environment has been solved.

Double DQN turned ON, Dueling DQN turned ON, and Prioritized Experience Replay turned ON solved the environment in 1380 episodes

Double DQN turned ON, Dueling DQN turned ON, and Prioritized Experience Replay turned OFF solved the environment in 747 episodes.

Double DQN turned ON, Dueling DQN turned OFF, and Prioritized Experience Replay turned OFF solved the environment in 640 episodes.

## Ideas for Future Work
Here's a list of optimizations that can be applied to the project:
1. Noisy Networks for Exploration [arxiv](https://arxiv.org/abs/1706.10295)
2. A Distributional Perspective on Reinforcement Learning [arxiv](https://arxiv.org/pdf/1707.06887.pdf)
3. Rainbow: Combining Improvements in Deep Reinforcement Learning [arxiv](https://arxiv.org/abs/1710.02298)
4. Distributional Reinforcement Learning with Quantile Regression [arxiv](https://arxiv.org/pdf/1710.10044.pdf)
5. Hierarchical Deep Reinforcement Learning [arxiv](https://arxiv.org/abs/1604.06057)
6. Neural Episodic Control [arxiv](https://arxiv.org/pdf/1703.01988.pdf)

Another idea would be to build a NN that will optimize hyperparameters and neural network structure for each model since it's time consuming to do it manually.
