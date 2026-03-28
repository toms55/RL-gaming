# Project 18: Evolutionary Reward Shaping for Reinforcement Learning Agents
**Course:** UTS 41004 AI/Analytics Capstone Project (Semester 1, 2026)
**Team:** Adam Cameron, Shifali Lakshmanan, Pak Hei Lee, Thomas Storey, Daniel James Martirosov
**Supervisor:** Dr. Mir Md. Jahangir Kabir

---

## Project Overview
This project investigates the use of Genetic Algorithms (GAs) to automatically generate and optimise reward functions for reinforcement learning agents, reducing reliance on manual reward engineering. Agents are trained using Q-Learning and Deep Q-Networks (DQN) across Gymnasium and MiniGrid benchmark environments, with performance compared between manually designed and evolutionarily derived reward functions.

---

## Repository Structure
```
RL-gaming/
├── notebooks/        # Jupyter notebooks for all experiments
├── results/          # Generated CSVs and plots (not tracked by Git)
├── logs/             # SB3 training logs (not tracked by Git)
├── requirements.txt  # Python dependencies
└── README.md
```

---

## Setup Instructions
### Prerequisites
- Python 3.10 or later
- Git

### Local Setup (Windows)
```bash
git clone https://github.com/toms55/RL-gaming.git
cd RL-gaming
py -3.10 -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python -m ipykernel install --user --name=AICproject18 --display-name "AIC Project 18 (Python 3.10)"
```

### Local Setup (Linux / macOS)
```bash
git clone https://github.com/toms55/RL-gaming.git
cd RL-gaming
python3.10 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python -m ipykernel install --user --name=AICproject18 --display-name "AIC Project 18 (Python 3.10)"
```

### Google Colab Setup
Open the desired notebook in Colab, uncomment the installation cell in Section 1, run it, restart the runtime (Runtime > Restart runtime), then run all remaining cells from Section 2 onwards. No other changes are needed.

---

## Notebooks
| Notebook | Description |
|---|---|
| `notebooks/baseline_rl.ipynb` | Baseline RL agent implementations across all environments |

---

## Dependencies
All dependencies are listed in `requirements.txt`. Key libraries:
| Library | Purpose |
|---|---|
| `stable-baselines3` | DQN agent implementation |
| `gymnasium` | CartPole and LunarLander environments |
| `minigrid` | MiniGrid grid-world environments |
| `torch` | Neural network backend for DQN |
| `pandas`, `matplotlib`, `seaborn` | Data logging and visualisation |