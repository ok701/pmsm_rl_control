## Reinforcement Learning Training

Train the model to obtain a customized agent. A **pre-trained agent** is also provided for convenience.

The following plot shows how varying the reward coefficients affects performance under **high-load conditions**:

<img src="./sim_data/agent/reward_var.png" width="700">

- Red line: Reference Speed  
- Green line: $Q_1, Q_2 = 10$, $R = 0.1$  
- Yellow line: $Q_1, Q_2 = 50$, $R = 0.5$  
- Blue line: $Q_1, Q_2 = 5$, $R = 0.1$



### Parameter Tuning

You can train and test with various parameters, such as:
- Motor parameters  
- Load torque  
- Training more or less reference speed values  
- Reward function structure  

Try adjusting them to see how they influence training outcomes.

From experience, handling **diverse load conditions** using **current-mode RL** is not significantly effective compared to **conventional PI control**.  
A **hybrid approach** combining RL with a **PI controller** in **speed mode** demonstrated **meaningfully improved performance**.
