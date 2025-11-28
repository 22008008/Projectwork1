## AI-Based Safe and Sustainable Traffic Signal System

Urban traffic congestion poses a significant challenge to modern cities, causing increased travel time, fuel consumption,and CO2 emissions. Traditional fixed-time signal systems are
inefficient because they cannot adapt to real-time changes in traffic conditions. This paper proposes an Artificial Intelligence (AI)-based smart and sustainable traffic signal system using Reinforcement Learning (RL). The proposed model integrates three major innovations: (1) Emergency Vehicle Priority, providing immediate green passage for ambulances and fire trucks; (2)
a CO2/Fuel-Aware Reward Function to reduce emissions and optimize fuel consumption; and (3) a Double Deep Q-Network with Prioritized Experience Replay (DDQN + PER) for stable and efficient learning. The system is implemented using SUMO simulation and Python via the TraCI interface. Experimental results demonstrate that the proposed model significantly reduces average waiting time, queue length, and CO2 emissions compared to conventional traffic controllers. The system thus provides a scalable, eco-friendly, and safety-oriented solution for intelligent urban traffic management.Index Terms—Reinforcement Learning, Traffic Signal Optimization, Emergency Vehicle Priority, Sustainable Transportation, DDQN, Prioritized Experience Replay, SUMO Simulation.

## About
Traffic congestion remains one of the most pressing urban issues, leading to delays, air pollution, and safety risks.Conventional traffic signal systems operate on predefined cycles and fail to handle dynamic traffic variations effectively.Adaptive traffic control systems have improved performance but remain limited in scalability and energy efficiency.Recent advancements in Artificial Intelligence (AI) and Reinforcement Learning (RL) offer promising solutions for intelligent traffic signal control. RL enables systems to learn optimal strategies by interacting with the environment and receiving rewards based on performance. Unlike rule-based methods, RL adapts in real time to changing conditions,learning from experience to improve performance.This paper presents an AI-based Safe and Sustainable Traffic Signal system that leverages RL to enhance road safety and minimize environmental impact. The proposed model introduces a hybrid DDQN + PER approach for faster and more stable training, integrates emergency vehicle Prioritization for critical response scenarios, and optimizes traffic flow while reducing emissions. The proposed framework aims to contribute to sustainable smart cities by balancing mobility,safety, and environmental responsibility

## Features

The system integrates three major innovations to provide a smart and sustainable solution to urban traffic challenges:

Advanced DRL Algorithm: Employs Double Deep Q-Network with Prioritized Experience Replay DDQN+PER for stable and efficient policy learning.

Multi-Objective Optimization: Uses a CO2/Fuel-Aware Reward Function to minimize traffic congestion (queue length) and environmental impact (emissions).

Safety Priority: Includes an Emergency Vehicle Priority module that provides immediate green passage for ambulances and fire trucks.

Adaptive Control: Dynamically adjusts signal timings based on real-time traffic conditions, eliminating the inefficiency of fixed-time systems.

## Requirements
Operating System: Requires a 64-bit OS (Windows 10 or Ubuntu) for compatibility with deep learning frameworks.

Development Environment: Python 3.6 or later is necessary for coding the Reinforcement Learning agent and TraCI interface.

Deep Learning Frameworks: TensorFlow (or PyTorch) for DDQN model training, SUMO (Simulation of Urban Mobility) for the environment.

Simulation Interface: TraCI (Traffic Control Interface) is essential for real-time communication between Python and SUMO.

Data Processing Libraries: NumPy and Pandas for efficient state/reward calculation and result analysis.

Version Control: Implementation of Git for collaborative development and effective code management.

IDE: Use of VSCode as the Integrated Development Environment for coding, debugging, and version control integration.

Additional Dependencies: Includes sumolib, traci, tensorflow, and numpy for simulation and deep learning tasks.

## System Architecture

The system architecture is built on a standard Reinforcement Learning framework, where the DDQN+PER agent learns from the SUMO environment via the TraCI interface.Reinforcement Learning Architecture FlowchartKey Interaction Loop:Environment (SUMO) sends the current State (queue length, traffic flow, emissions) via TraCI to the Agent.Agent DDQN+PER processes the state and chooses the optimal Action (signal phase change).Agent sends the Action command back to SUMO via TraCI.SUMO executes the phase change and calculates the new Reward (based on queue length and CO2.Agent uses the new state and reward to Update its policy network weights.

<img width="631" height="632" alt="Screenshot 2025-10-12 172020" src="https://github.com/user-attachments/assets/fd514235-c991-435d-b34b-ee16dc5ab9ea" />



**UML Diagram :**

<img width="1402" height="709" alt="Screenshot 2025-11-28 131915" src="https://github.com/user-attachments/assets/1fbb09de-7c7b-4f0f-ae79-78d4df8c245b" />

**Flow Chart :** 

<img width="1435" height="460" alt="Screenshot 2025-11-28 130229" src="https://github.com/user-attachments/assets/b9fe73cf-a048-4f54-be56-0d672f30b684" />

## Output

<!--Embed the Output picture at respective places as shown below as shown below-->
**A. Output and Results**

<img width="1232" height="719" alt="Screenshot 2025-11-28 135731" src="https://github.com/user-attachments/assets/955ff5c4-ae24-4a20-9a38-ed03eef5b624" />

This chart validates the efficiency and sustainability of the $\text{DDQN}+\text{PER}$ model by comparing it against Fixed-Time and standard $\text{DQN}$ baselines.

**B. Test Cases and Validation**

<img width="1442" height="220" alt="Screenshot 2025-11-28 135739" src="https://github.com/user-attachments/assets/a2fbe868-1d26-4bfe-a73f-a5bab5ea359d" />

TC-1 (Balanced Peak Hour Load): Successfully demonstrated the lowest congestion and emissions metrics, proving core adaptive efficiency.

TC-2 (Emergency Vehicle Protocol): Confirmed near-zero delay for the priority vehicle, validating the critical override logic.

TC-3 (Highly Unbalanced Flow): The agent adapted by allocating proportionally more green time to the congested roads, preventing gridlock.

## Results and Impact
The system successfully addresses the core problems of urban congestion and environmental pollution.Enhanced Urban Mobility: The $28\%$ reduction in average waiting time significantly improves travel efficiency for commuters.Environmental Sustainability: The $18\%$ reduction in $\text{CO}_2$ emissions directly contributes to cleaner air and aligns with urban sustainability goals.Improved Safety: The integration of the Emergency Vehicle Priority module ensures that safety-critical services face minimal delays, saving time and potentially lives.Foundation for Smart Cities: The project provides a smart and scalable solution based on Deep Reinforcement Learning, positioning it as an integral component for future Intelligent Transportation Systems (ITS).

This project serves as a strong foundation for future developments in Smart City infrastructure and contributes to creating a more efficient, inclusive, and environmentally responsible urban environment.



## Articles published / References
1 . K. Gupta, R. Jain, V. Kumar, “Multi-Agent DDQN with Prioritized Experience Replay for Traffic Signal Optimization,” IET Intelligent Transport Systems, vol. 18, no. 1, pp. 77–89, 2024.

2 . J. Chen, H. Wei, Z. Li, “HiLight: Hierarchically and Cooperatively Learning Traffic Signal Control,” AAAI Conference on Artificial Intelligence, pp. 612–620, 2021.

3 . B. Xu, K. Li, P. Wang, “HumanLight: RL-Based Person-Throughput Optimization for Urban Traffic Signals,” Berkeley Press, vol. 7, 2024.

4 . R. Zhou, X. Yu, C. Chen, “Constrained Traffic Signal Control Under Competing Public Transport Priorities Using Safe RL,” Transportation Research Part C, vol. 168, 2025.

5 . G. Lee, D. Jung, M. Park, “RUTGe: Realistic Urban Traffic Generator for RL-Based Control,” IEEE Trans. Intelligent Transport Systems, vol. 26, 2025.



