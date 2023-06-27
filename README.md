# Reinforcement Learning: N-Step SARSA and λ-SARSA

This code implements the N-Step SARSA and λ-SARSA algorithms for reinforcement learning in the WindyGridworld environment.

## Environment

The `WindyGridworld` class represents the Windy Gridworld environment. It is a grid with a start state, a goal state, and wind effects in certain columns. The agent can take actions to move in the grid, and the goal is to reach the goal state while minimizing the number of steps and avoiding obstacles.

## Algorithms

The code implements the following algorithms:

### N-Step SARSA

The `n_step_sarsa` function implements the N-Step SARSA algorithm. It takes the following parameters:
- `env`: The environment object representing the Windy Gridworld.
- `n`: The number of steps to look ahead for updates.
- `alpha`: The learning rate.
- `gamma`: The discount factor.
- `epsilon`: The exploration rate.
- `num_episodes`: The number of episodes to run the algorithm.

The function returns the learned Q-values, episode rewards, and episode lengths.

### λ-SARSA

The `lambda_sarsa` function implements the λ-SARSA algorithm. It takes similar parameters as the N-Step SARSA algorithm, including an additional parameter `lmbda` representing the eligibility trace decay rate.

The function returns the learned Q-values, episode rewards, and episode lengths.

## Running the Code

To run the code, follow these steps:
1. Create an instance of the WindyGridworld environment.
2. Set the algorithm parameters such as learning rate, discount factor, exploration rate, and the number of episodes.
3. Call the desired algorithm function (`n_step_sarsa` or `lambda_sarsa`) with the environment and parameters.
4. Plot the learning curves to visualize the algorithm's performance.

You can modify the algorithm parameters and experiment with different settings to observe their impact on learning.

For detailed implementation and usage examples, refer to the code comments.

