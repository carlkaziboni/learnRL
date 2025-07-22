# LearnRL 🤖🎮

This repository contains my notebooks and projects from completing the [Hugging Face Deep Reinforcement Learning Course](https://huggingface.co/learn/deep-rl-course). Through this course, I gained hands-on experience with modern RL algorithms and trained agents across diverse environments.

## 🗂️ Repository Structure

```
learnRL/
├── unit1.ipynb           # Introduction to Deep RL
├── bonus_unit1.ipynb     # Additional Unit 1 exercises
├── unit2.ipynb           # Q-Learning fundamentals  
├── unit3.ipynb           # Deep Q-Networks (DQN)
├── unit4.ipynb           # Policy Gradient Methods
├── unit5.ipynb           # Actor-Critic Methods
├── unit6.ipynb           # Proximal Policy Optimization (PPO)
├── unit8_part1.ipynb     # Multi-Agent RL (Part 1)
├── unit8_part2.ipynb     # Multi-Agent RL (Part 2)
└── MARLAgents.ipynb      # Multi-Agent RL with Agents
```

## 📚 Notebooks Overview

### Core Course Units
- **`unit1.ipynb`** - Introduction to Deep RL and the RL framework (PPO on LunarLander-v2)
- **`bonus_unit1.ipynb`** - Additional exercises and deep dives from Unit 1
- **`unit2.ipynb`** - Q-Learning with Taxi-v3 environment
- **`unit3.ipynb`** - Deep Q-Networks (DQN) with Space Invaders
- **`unit4.ipynb`** - REINFORCE on CartPole-v1 and Pixelcopter
- **`unit5.ipynb`** - PPO with Unity ML-Agents (SnowballTarget & Pyramids)
- **`unit6.ipynb`** - A2C for robotics with PandaReachDense

### Advanced Topics  
- **`unit8_part1.ipynb`** - PPO parameter investigation with LunarLander-v2
- **`unit8_part2.ipynb`** - Custom RL in VizDoom health gathering environment
- **`MARLAgents.ipynb`** - Multi-Agent RL with POCA algorithm on SoccerTwos

### Fundamentals
- **Markov Decision Processes (MDPs)**
- **Value-based methods** (Q-Learning, DQN, Double DQN)
- **Policy-based methods** (REINFORCE, Actor-Critic)
- **Advanced algorithms** (PPO, A2C, SAC)

## 🚀 Key Topics Covered
- **Classic Control** (CartPole, MountainCar)
- **Atari Games** (Breakout, Space Invaders)
- **Robotics Simulations** (PyBullet environments)
- **Custom Environments** using Gymnasium

### Libraries & Frameworks
- **Stable-Baselines3** for algorithm implementations
- **Gymnasium** for environment management
- **Hugging Face Hub** for model sharing
- **WandB** for experiment tracking
- **PyTorch** for deep learning components

## 📋 Prerequisites

```bash
# Core dependencies
pip install gymnasium[classic_control,atari]
pip install stable-baselines3[extra]
pip install huggingface_hub
pip install wandb
pip install torch torchvision
pip install jupyter notebook
```

## 🔧 Setup Instructions

1. **Clone the repository:**
```bash
git clone https://github.com/carlkaziboni/learnRL.git
cd learnRL
```

2. **Create a virtual environment:**
```bash
python -m venv rl_env
source rl_env/bin/activate  # On Windows: rl_env\Scripts\activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Set up Hugging Face authentication:**
```bash
huggingface-cli login
```

## 📖 How to Use

Each unit contains Jupyter notebooks with:
- **Theory explanations** and mathematical foundations
- **Code implementations** with detailed comments
- **Training scripts** for various algorithms
- **Evaluation metrics** and performance analysis
- **Trained models** ready for testing

### Running a Notebook
```bash
# Start with the introduction
jupyter notebook unit1.ipynb

# Or explore Q-Learning fundamentals
jupyter notebook unit2.ipynb

# Try advanced multi-agent scenarios
jupyter notebook MARLAgents.ipynb
```

### Training Models
Each notebook contains complete training loops and you can run them cell by cell to:
- Understand the theory behind each algorithm
- Train agents on various environments
- Visualize training progress and results
- Save and load trained models

## 🎯 Key Achievements

- ✅ **Completed all 8 units** of the Hugging Face Deep RL Course
- ✅ **Mastered CartPole-v1** with perfect score (500/500) using REINFORCE
- ✅ **Conquered Space Invaders** with 430.6 average score using DQN
- ✅ **Successfully trained agents** across 11 different environments
- ✅ **Deployed all models** to Hugging Face Hub with passing scores
- ✅ **Explored Multi-Agent RL** with complex cooperative scenarios

## 📊 My Training Results

| Unit | Algorithm | Environment | Min Score | **Best Score** | Model |
|------|-----------|-------------|-----------|----------------|-------|
| **Unit 1** | PPO | LunarLander-v2 | 200 | **240.36** | [ppo-LunarLander-v1](https://huggingface.co/carlkaziboni/ppo-LunarLander-v1) |
| **Unit 2** | Q-Learning | Taxi-v3 | 4 | **4.58** | [Taxi-v3](https://huggingface.co/carlkaziboni/Taxi-v3) |
| **Unit 3** | DQN | SpaceInvadersNoFrameskip-v4 | 200 | **430.6** | [dqn-SpaceInvadersNoFrameskip-v4](https://huggingface.co/carlkaziboni/dqn-SpaceInvadersNoFrameskip-v4) |
| **Unit 4** | REINFORCE | CartPole-v1 | 350 | **500** 🎯 | [Reinforce-v2](https://huggingface.co/carlkaziboni/Reinforce-v2) |
| **Unit 4** | REINFORCE | Pixelcopter-PLE-v0 | 5 | **17.77** | [Reinforce-v1](https://huggingface.co/carlkaziboni/Reinforce-v1) |
| **Unit 5** | PPO | ML-Agents-SnowballTarget | -100 | **0** | [ppo-SnowballTarget](https://huggingface.co/carlkaziboni/ppo-SnowballTarget) |
| **Unit 5** | PPO | ML-Agents-Pyramids | -100 | **0** | [ppo-PyramidsRND](https://huggingface.co/carlkaziboni/ppo-PyramidsRND) |
| **Unit 6** | A2C | PandaReachDense | -3.5 | **-0.30** | [a2c-PandaReachDense-v3](https://huggingface.co/carlkaziboni/a2c-PandaReachDense-v3) |
| **Unit 7** | POCA | ML-Agents-SoccerTwos | -100 | **0** | [poca-SoccerTwos](https://huggingface.co/carlkaziboni/poca-SoccerTwos) |
| **Unit 8 PI** | PPO | LunarLander-v2 | -500 | **-174.23** | [ppo-LunarLander-v2](https://huggingface.co/carlkaziboni/ppo-LunarLander-v2) |
| **Unit 8 PII** | Custom | doom_health_gathering_supreme | 5 | **5.2** | [rl_course_vizdoom_health_gathering_supreme](https://huggingface.co/carlkaziboni/rl_course_vizdoom_health_gathering_supreme) |

### 🏆 Standout Performances
- **Perfect CartPole Solution**: Achieved maximum possible score of 500 with REINFORCE
- **Atari Mastery**: Strong performance on Space Invaders with 430.6 average score  
- **Robotics Success**: Significant improvement in PandaReachDense from -3.5 to -0.30
- **Multi-Agent Coordination**: Successfully trained cooperative agents in team-based environments

---

*Repository showcasing my journey through deep reinforcement learning fundamentals to advanced multi-agent scenarios.*
