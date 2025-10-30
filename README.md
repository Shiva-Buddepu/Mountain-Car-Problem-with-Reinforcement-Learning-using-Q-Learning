#  Mountain Car Problem with Reinforcement Learning using Q-Learning

This project demonstrates how a **Q-Learning agent** can learn to solve the classic **MountainCar-v0** environment from OpenAI Gym.  
The objective is for the car to reach the top of the hill using learned behavior rather than random actions through **Reinforcement Learning**.

---

##  Project Overview

The **MountainCar-v0** environment is a fundamental reinforcement learning task where an underpowered car must climb a steep hill.  
Since the car’s engine is not strong enough to reach the goal directly, it must build momentum by moving back and forth strategically.  
This project applies **Q-Learning**, a value-based reinforcement learning algorithm, to train the agent to achieve this task efficiently.

---

##  What is Q-Learning?

**Q-Learning** is a model-free reinforcement learning algorithm that learns the optimal action-value function **Q(s, a)** through trial and error, using the Bellman equation:

\[
Q(s, a) = Q(s, a) + \alpha [r + \gamma \max_{a'} Q(s', a') - Q(s, a)]
\]

Where:
- **s** → Current state  
- **a** → Action taken  
- **r** → Reward received  
- **s'** → Next state  
- **α (alpha)** → Learning rate  
- **γ (gamma)** → Discount factor  

---
## ⚙️ Project Steps

1. **Setup and Dependencies**
   ```bash
   !pip install gym Box2D gymnasium[classic-control] moviepy imageio ffmpeg pyvirtualdisplay swig

2. **Initialize the Environment**

Create the MountainCar-v0 environment using Gym.

Inspect its observation space, action space, and reward structure.

3. **Random Agent Baseline**

Run a random agent to establish a performance benchmark.

Record episode rewards and visualize results.

4. **Q-Learning Implementation**

Discretize the continuous state space into bins.

Initialize the Q-table with zeros.

Use an ε-greedy policy for exploration vs exploitation.

Update Q-values based on experience.

5. **Performance Visualization**

Plot total rewards and actions per episode to track learning progress.

Capture the agent’s movement and generate a video (cassietvid.mp4).



