# labo-03-jumper-Tjorven-Verbeeck
## Description
1. Set-up: A linear movement task where the agent must jump to dodge a moving wall.
2. Goal: Jump over 5 consecutive walls without getting hit.
3. Agents: The environment contains one agent.
4. Agent Reward Function: 
    1. -0.05 for each jump
    2. -1 for hitting the moving wall.
    3. +1.0 for jumping over wall.
5. Behavior Parameters: 
    1. Vector Observation space: One variable corresponding to current state, one variable corresponding to the wall state.
    2. Actions: 1 discrete action branch with 2 actions (jump, do nothing).
    3. Visual Observations: Ray Perception Sensor 3D, 
6. Float Properties: None
7. Benchmark Mean Reward: 0.98

## Course of training:
The training was fairly slow because it had to come from a negative value. At 200000 steps, the model was actually fully trained. After this, there were some down moments where the model returned to making some more errors. I think this is because the model had returned to the discovery phase.
I also modified my .yml file. Among other things, I increased the number of steps here to 1000000 as shown in the image above.
