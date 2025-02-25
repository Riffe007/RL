Original Project: Augmented Random Search (ARS) Reinforcement Learning (RL) Framework

📌 Overview

This project is an Augmented Random Search (ARS) reinforcement learning implementation, focused on training robotic agents in PyBullet environments. It includes custom-built environments, robot locomotion simulators, and manually implemented ARS-based policy updates using NumPy.

The framework is designed for continuous control tasks, such as locomotion and robotic manipulation, using a simple linear policy gradient update approach.

🚀 Features

✅ ARS-based RL Training – Implements Augmented Random Search to optimize policies.✅ Custom PyBullet Environments – Includes locomotion and robotic manipulation simulations.✅ Manual State Normalization – Uses a custom normalizer to stabilize training.✅ Single-Threaded Execution – Training runs in a single process.✅ Basic Logging System – Uses print() statements for monitoring performance.✅ Hardcoded Gym Wrappers – Custom environment wrappers for Gym and PyBullet.

📂 Directory Structure
```plaintext
ARS-RL-Project/
│── agents/                     # ARS RL Training Code
│   ├── ars.py                  # Main ARS Algorithm
│
│── environments/                # PyBullet-based Custom Environments
│   ├── env_bases.py
│   ├── gym_locomotion_envs.py
│   ├── gym_manipulator_envs.py
│   ├── gym_pendulum_envs.py
│
│── robots/                      # Custom Robot Models
│   ├── robot_bases.py
│   ├── robot_locomotors.py
│   ├── robot_manipulators.py
│   ├── robot_pendula.py
│
│── scenes/                      # Simulation Scenes
│   ├── scene_abstract.py
│   ├── scene_stadium.py
│
│── tools/                       # Additional Helpers
│   ├── kerasrl_utils.py         # Keras RL integration
│
│── logs/                        # Training Logs
│
│── brs/monitor/                 # Performance Monitoring
│
│── README.md                    # Documentation
```
💾 Installation

pip install numpy gym pybullet

🛠️ Usage

Run ARS training on HalfCheetahBulletEnv:

python agents/ars.py

🔬 Limitations

🚫 Outdated PyBullet-based environments (Gymnasium/MuJoCo are now standard).

🚫 No parallelization or multi-GPU support (single-threaded).

🚫 No advanced RL techniques (pure ARS, no PPO/SAC).

🚫 Logging is minimal (no TensorBoard, WandB).
