# Blackjack Neural Network Analysis

A large-scale simulation and machine learning project exploring blackjack strategy optimization using NeuroEvolution of Augmenting Topologies (NEAT), evolutionary algorithms, and comparative AI experimentation.

## Project Overview

This project investigates whether evolutionary neural networks can develop more effective blackjack decision strategies than deterministic rule-based approaches through large-scale simulation and iterative optimization.

The project includes:

* A fully simulated blackjack environment built in Python
* Neuroevolutionary AI training using NEAT-Python
* Large-scale simulation testing across millions of blackjack hands
* Comparative A/B testing between evolved neural networks and baseline rule-based agents
* Neural-network topology visualization and performance analysis
* Experimental evaluation of strategy convergence and win-rate optimization

The goal of the project was not only to improve blackjack strategy performance, but also to explore machine learning experimentation workflows, simulation modeling, evolutionary optimization, and AI-driven decision systems.

---

# Key Features

## Blackjack Simulation Environment

* Custom blackjack game engine built entirely in Python
* Automated dealer/player logic
* Multi-round simulation support
* Configurable gameplay and training parameters
* Simulation-ready architecture for large-scale experimentation

## NeuroEvolution with NEAT

Implemented NeuroEvolution of Augmenting Topologies (NEAT) to:

* Evolve neural-network architectures
* Optimize blackjack decision-making strategies
* Select high-performing genomes through fitness-based evolution
* Experiment with topology growth and behavioral adaptation over generations

## Large-Scale Simulation Testing

* Simulated millions of blackjack hands
* Compared evolved AI agents against deterministic rule-based baseline agents
* Evaluated win-rate performance and convergence behavior
* Conducted repeated simulation runs for comparative analysis

## A/B Strategy Testing

Designed controlled simulation experiments comparing:

* NEAT-evolved neural-network agents
* Rule-based blackjack AI agents

The evolved neural-network strategies achieved approximately:

3.25% improvement in win rate compared to the base strategy.

over the baseline rule-based strategy during testing.

## Model Visualization & Analysis

* Serialized trained models using Pickle
* Visualized neural-network topologies and architecture evolution
* Analyzed strategy convergence and behavioral adaptation
* Evaluated performance trends across generations

---

# Technologies Used

## Languages & Libraries

* Python
* pandas
* NumPy
* NEAT-Python
* Pickle

## Machine Learning Concepts

* NeuroEvolution
* Evolutionary Algorithms
* Fitness-Based Optimization
* Neural Networks
* Simulation Modeling
* Comparative A/B Testing

## Analytical Concepts

* Experimental Design
* Statistical Comparison
* Performance Analysis
* Strategy Optimization
* Convergence Analysis

---

# Project Structure

```text
Blackjack_Neural_Network_Analysis/
│
├── Configs/                # NEAT configuration files
├── Checkpoints/            # Saved training checkpoints
├── Visualizations/         # Generated topology graphs and outputs
├── Data/                   # Simulation result datasets
├── blackjack.py            # Blackjack game environment
├── train.py                # NEAT training pipeline
├── evaluate.py             # Model evaluation/testing
├── visualize.py            # Network visualization utilities
├── requirements.txt
└── README.md
```

---

# How It Works

## 1. Blackjack Simulation

The blackjack engine simulates complete gameplay cycles including:

* card dealing,
* player actions,
* dealer logic,
* win/loss evaluation,
* bankroll outcomes.

The simulation environment provides the feedback loop required for evolutionary training.

## 2. Neural Network Inputs

The AI agent receives game-state information such as:

* player hand value,
* dealer visible card,
* usable ace state,
* additional gameplay conditions.

The neural network outputs gameplay decisions such as:

* hit,
* stand,
* or other configured actions.

## 3. Evolutionary Training

Using NEAT:

* populations of neural networks are generated,
* networks compete through blackjack simulations,
* fitness scores are assigned based on performance,
* higher-performing genomes survive and evolve,
* architectures become increasingly optimized across generations.

## 4. Comparative Evaluation

The evolved AI strategies are benchmarked against deterministic rule-based agents through repeated simulation testing and win-rate analysis.

---

# Example Workflow

```python
# Train NEAT population
python train.py

# Resume from checkpoint
python train.py --checkpoint

# Evaluate trained model
python evaluate.py

# Visualize network topology
python visualize.py
```

---

# Results & Findings

Key observations from experimentation included:

* Evolutionary neural networks successfully learned competitive blackjack strategies through simulation-based optimization.
* Evolved strategies demonstrated measurable win-rate improvements over baseline deterministic approaches.
* Neural-network architectures adapted over generations to optimize gameplay decision patterns.
* Large-scale simulation testing provided valuable insight into convergence behavior and strategy stability.

---

# Challenges & Lessons Learned

This project involved several engineering and analytical challenges, including:

* Managing computationally intensive long-running simulations
* Checkpoint recovery and model persistence
* Balancing evolutionary fitness functions
* Preventing premature convergence
* Evaluating noisy simulation outcomes
* Designing scalable experimentation workflows

The project provided hands-on experience with:

* machine learning experimentation,
* simulation modeling,
* evolutionary optimization,
* analytical evaluation,
* and AI system design.

---

# Future Improvements

Potential future enhancements include:

* Additional blackjack actions (split, double down, insurance)
* Reinforcement learning comparison models
* GPU-accelerated simulation workflows
* Hyperparameter optimization
* More advanced statistical evaluation metrics
* Interactive dashboard visualization of training performance
* Parallelized simulation execution

---



