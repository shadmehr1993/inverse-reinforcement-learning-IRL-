
## Inverse Reinforcement Learning (IRL) Agent for HVAC Control
This repository includes a simplified implementation of an **Inverse Reinforcement Learning (IRL) agent** for supervisory control of HVAC systems in district buildings.
The objective of IRL is to **infer the underlying reward function** that explains the behavior of an expert controller. In this project, expert demonstrations are generated using a **rule-based control (RBC) strategy** operating within a district energy simulation environment.
Using the recorded expert trajectories (state–action pairs), the IRL framework estimates a reward structure that captures the implicit trade-off between:
* energy consumption
* operational cost
* thermal comfort
* system stability
Once the reward function is learned, a control policy is optimized to reproduce or improve upon the expert behavior.
The state representation used by the IRL agent includes several operational variables such as:
* supply water temperature
* return water temperature
* outdoor temperature
* cooling demand
* photovoltaic (PV) generation
* electricity price signals
The policy network outputs continuous control actions including:
* supply water temperature setpoints
* pump mass flow rate
* storage operation decisions

⚠️ **Note:**
This repository provides a **partial implementation of the IRL agent** used in the research project. The full experimental framework, including the complete co-simulation environment and additional control strategies, is described in the associated publication.
The shared code focuses on demonstrating the **methodological workflow of IRL for HVAC control**, enabling researchers and practitioners to explore imitation-based learning approaches for building energy management.


<img width="1090" height="521" alt="image" src="https://github.com/user-attachments/assets/45ebc826-afd0-453a-81b8-8cf431b1376c" />
