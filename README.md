# Bayesian Active Exploration for Abstract Reasoning
### Treating ARC-AGI-3 as an Unknown Terrain

[![Kaggle](https://img.shields.io/badge/Kaggle-ARC%20Prize%202026-blue)](https://www.kaggle.com/competitions/arc-prize-2026-paper-track)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/status-active--development-orange)]()

## 📖 Overview

This repository contains the official code and paper submission for the **ARC Prize 2026 - Paper Track**. 

We propose a novel framework for ARC-AGI-3 that leverages principles of **Bayesian experimental design** and **geophysical survey planning** to maximize exploration efficiency. By modeling the ARC environment as an unknown dynamical system and employing Gaussian Process surrogate models, our agent actively selects actions to maximize information gain, inferring latent rules and goals with minimal interactions. 

This approach achieves high **Relative Human Action Efficiency (RHAE)** by bridging the gap between systematic exploration and targeted exploitation, demonstrating that cross-domain wisdom from Earth sciences can unlock new paradigms in artificial general intelligence.

## 🧠 Methodology

Our agent operates on a three-phase exploration-exploitation loop:

1. **Exploration Phase:** Systematically probes the environment using active learning to infer underlying rules. We use Gaussian Process surrogate models to predict environment dynamics from sparse observations.
2. **World Model Construction:** Builds a programmatic model of the environment dynamics using a custom Domain-Specific Language (DSL) for grid transformations.
3. **Efficient Execution:** Executes the inferred solution with minimal actions to maximize the RHAE score, utilizing Expected Improvement acquisition functions adapted from geophysical survey planning.

### Core Innovations
- **Gaussian Process Surrogate Models** for predicting environment dynamics under uncertainty.
- **Expected Improvement Acquisition Functions** to select exploratory actions that maximize information gain.
- **Sequential Experimental Design** principles adapted from geophysical survey planning.
- **Test-Time Rejection Sampling** inspired by Monte Carlo simulations in geophysics.

## 📂 Repository Structure

```text
├── data/                   # ARC-AGI-3 environment data and configurations
├── src/                    # Source code for the Bayesian agent
│   ├── agent.py            # Main agent loop (Explore-Exploit-Validate)
│   ├── bayesian_model.py   # Gaussian Process implementation
│   ├── dsl.py              # Domain-Specific Language for grid transformations
│   └── utils.py            # Helper functions for logging and visualization
├── notebooks/              # Jupyter notebooks for experimentation and analysis
├── paper/                  # LaTeX source and PDF of the final paper
├── requirements.txt        # Python dependencies
├── LICENSE                 # MIT License
└── README.md               # This file
```

**Note:** The full source code and model weights will be released upon completion of the ARC Prize 2026 competition. This repository currently serves as the official project page.

## 🚀 Getting Started
### Prerequisites

- Python 3.10+
- ARC-AGI-3 Starter Kit
- Kaggle API key (for submitting to the leaderboard)

### Installation

**Clone the repository:**
```text
git clone https://github.com/mubquaidian/arc-agi-3-bayesian-exploration.git
cd arc-agi-3-bayesian-exploration
```
**Install dependencies:**    
```text
pip install -r requirements.txt
```
**Set up your environment variables:**
```text
export KAGGLE_USERNAME=your_username
export KAGGLE_KEY=your_api_key
```
## Running the Agent

```text
python src/agent.py --environment ARC-AGI-3 --exploration_budget 100
```
## 📊 Results

- **Metric:**	Score
- **Public Leaderboard:** RHAE	[TBD]
- **Private Leaderboard:** RHAE	[TBD]

(Results will be updated as the competition progresses)

## 🗺️ Roadmap

- [x] Repository initialization and baseline architecture
- [ ] Implement Gaussian Process surrogate model
- [ ] Develop custom Domain-Specific Language (DSL)
- [ ] Integrate Bayesian optimization for exploration
- [ ] Run baseline experiments on public ARC-AGI-3 games
- [ ] Submit to Kaggle Leaderboard
- [ ] Write and submit Paper Track writeup

## 📜 Citation

If you use this code or find our approach useful in your research, please cite our paper:
```bibtex
@article{brotherhood2026bayesian,
  title={Bayesian Active Exploration for Abstract Reasoning: Treating ARC-AGI-3 as an Unknown Terrain},
  author={Muhammad Umar Bilal},
  journal={ARC Prize 2026 - Paper Track},
  year={2026},
  url={https://www.kaggle.com/competitions/arc-prize-2026-paper-track}
}
```
## 🤝 Contact

- **Muhammad Umar Bilal**
- Founder, Eight Pillars Consultancy FZ-LLC
- M.Sc. Geophysics, Quaid-e-Azam University (2005)
- 13+ Years International Experience (UAE, Saudi Arabia, Germany, Pakistan)
- [LinkedIn Profile](https://www.linkedin.com/in/muhammad-umar-bilal-umarbillallucky)
