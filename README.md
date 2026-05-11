# flappy-bird-neat-ai
AI-powered Flappy Bird agent using NeuroEvolution of Augmenting Topologies (NEAT) for autonomous gameplay optimization

# Optimization of Flappy Bird Using NEAT

An AI-powered implementation of the classic Flappy Bird game using the NeuroEvolution of Augmenting Topologies (NEAT) algorithm. This project demonstrates how evolutionary algorithms can automatically design and optimize neural network architectures capable of learning complex sequential decision-making tasks without explicitly programmed rules.

## Project Overview

The objective of this project is to train an autonomous agent to play Flappy Bird by evolving neural networks over successive generations. Instead of manually defining the bird's behavior, the system uses NEAT to optimize both the network weights and topology based on gameplay performance.

This project was developed as my undergraduate final year thesis and explores the practical application of evolutionary computation, neural networks, and optimization algorithms.

## Key Features

- Manual Flappy Bird gameplay implementation
- AI agent trained using the NEAT algorithm
- Dynamic neural network topology evolution
- Fitness-based selection, mutation, and crossover
- Visualization of training progress
- Pre-trained model (`best.pickle`) included
- Configurable hyperparameters via `config-feedforward.txt`

## Tech Stack

|         Category       |       Technologies       |
|------------------------|--------------------------|
| Programming Language   |         Python           |
|    Game Development    |         Pygame           |
| Evolutionary Algorithm |       NEAT-Python        |
|   Data Visualization   |        Matplotlib        |
| Development Environment|     Jupyter Notebook     |


## Problem Statement

The objective of this project is to investigate whether an evolutionary algorithm can autonomously learn an effective strategy to play Flappy Bird. Rather than manually defining the bird's behavior, the system evolves neural network topologies and connection weights based solely on gameplay performance.

The broader goal is to explore how neuroevolution techniques can be applied to real-world optimization and autonomous decision-making problems.

## Methodology

### 1. Game Environment
A Flappy Bird simulator was implemented using Pygame.

### 2. Neural Network Inputs
Each genome receives:
- Bird's vertical position
- Distance to the next pipe
- Height of the top pipe
- Height of the bottom pipe

### 3. Output
The neural network produces a binary decision:
- `1` → Jump
- `0` → Do nothing

### 4. Fitness Function
Genomes are rewarded for:
- Surviving longer
- Successfully passing pipes

Genomes are penalized for collisions.

### 5. Evolution Process
The NEAT algorithm performs:
- Selection
- Mutation
- Crossover
- Speciation

The best-performing genomes are propagated to subsequent generations.

## Results

- Achieved a success rate of over **90%** across repeated evaluation runs.
- Significant performance improvements were observed within the first 20–30 generations.
- The evolved neural network successfully generalized across varying obstacle configurations.

## Real-World Applications

The techniques explored in this project are applicable to:

- Autonomous vehicles
- Robotics
- Drone navigation
- Adaptive control systems
- Game AI
- Optimization problems

## Repository Structure

```text
Flappy-Bird-With-NEAT-Algorithm/
├── .github/workflows/
├── DOCUMENTATIONS/
├── Visuals/
├── imgs/
├── Base Model Flappy Bird.ipynb
├── NEAT Algo Flappy Bird.ipynb
├── best.pickle
├── config-feedforward.txt
├── requirements.txt
├── test.py
└── README.md


## Installation

### Clone the Repository

```bash
git clone https://github.com/Shubhampatel001/Flappy-Bird-With-NEAT-Algorithm.git
cd Flappy-Bird-With-NEAT-Algorithm

## Usage

### Play the Game Manually

Open and run the following notebook:

```text
Base Model Flappy Bird.ipynb

## Configuration

The `config-feedforward.txt` file contains the hyperparameters used by the NEAT algorithm, including:

- Population size
- Mutation probabilities
- Compatibility threshold
- Activation functions
- Speciation settings

By modifying these parameters, different evolutionary behaviors and training outcomes can be explored.

## My Contributions

As part of my undergraduate final year thesis, I was actively involved in the following tasks:

- Studied the NEAT algorithm and its application to neuroevolution.
- Designed and implemented the fitness function used to evaluate genomes.
- Tuned hyperparameters to improve convergence and performance.
- Trained and evaluated the agent across multiple generations.
- Analyzed the results and documented key findings.
- Explored real-world applications of evolutionary algorithms in autonomous systems.

## Future Enhancements

Potential improvements to this project include:

- Parallelizing the training process to reduce execution time.
- Performing automated hyperparameter optimization.
- Comparing NEAT with Deep Q-Networks (DQN) and other reinforcement learning approaches.
- Deploying the project as an interactive web application.
- Extending the approach to more complex control and optimization problems.

## Academic Significance

This project strengthened my understanding of:

- Evolutionary computation
- Neural networks
- Optimization algorithms
- Reinforcement learning concepts
- Experimental research methodology

It also inspired my long-term interest in developing intelligent systems capable of autonomous decision-making in dynamic environments.

## References

1. Kenneth O. Stanley and Risto Miikkulainen, *Evolving Neural Networks Through Augmenting Topologies*, Evolutionary Computation, 2002.
2. NEAT-Python Documentation: https://neat-python.readthedocs.io/
3. Pygame Documentation: https://www.pygame.org/docs/

## License

This project is intended for academic and educational purposes.
