# DDPG on Cartpole Swingup (dm_control)

## Project Overview
This project trains a Deep Deterministic Policy Gradient (DDPG) agent on the dm_control Cartpole Swingup task using Stable-Baselines3, Shimmy, and Gymnasium wrappers. The objective is to swing the pole upward from the hanging position and balance it upright using continuous torque control. Training is performed across three different seeds, and the final results include training logs, evaluation videos, and a minimalist learning curve plot.

---

## Algorithm: DDPG
DDPG (Deep Deterministic Policy Gradient) is an off-policy actor–critic reinforcement learning algorithm designed for continuous action spaces. It uses:
- A deterministic actor network  
- A critic network to estimate Q-values  
- Gaussian noise for exploration  
- Target networks for stabilization  

DDPG is sensitive to hyperparameters but performs reasonably well on continuous control tasks like Cartpole Swingup.

---

## Training Setup
- Environment: `dm_control/cartpole-swingup-v0`
- Algorithm: DDPG
- Timesteps: ~200,000 per seed
- Seeds: `0`, `1`, `2`
- Noise: NormalActionNoise (σ = 0.1)

Outputs (modifiable later):
