# Flappy Bird AI with NEAT-Python

This repository contains a Flappy Bird game clone and an implementation of an AI that learns to play the game using the NEAT algorithm. The project is built using Python and the NEAT-Python library.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [How It Works](#how-it-works)
- [Results](#results)

## Introduction

This project demonstrates how to use NEAT, a genetic algorithm for evolving neural networks, to train an AI to play Flappy Bird. The AI learns through generations of simulated gameplay, improving over time by evolving its neural network topology.

## Features

- **Flappy Bird Game**: A clone of the popular Flappy Bird game implemented in Python.
- **AI Training**: Uses NEAT-Python to train an AI to play the game.
- **Visualization**: Real-time visualization of the game and the AI's learning progress.
- **Configurable**: Easily modify game parameters and NEAT settings.

## Installation

To get started, clone this repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/flappy-bird-ai-neat.git
cd flappy-bird-ai-neat
pip install -r requirements.txt
```
## Usage

To run the game and start the AI training process, use the following command:

```bash
python flappy_bird.py

This will launch the game window and begin the training process, where multiple AI agents will attempt to learn how to play Flappy Bird.
```

## Configuration

You can adjust the NEAT algorithm's settings by modifying the config_file.txt file. This file contains various parameters that control the evolution process, such as population size, mutation rates, and network structure.

## How It Works

1. **Initialization:** A population of random neural networks is created.
2. **Evaluation:** Each network controls a bird in the game, and its performance is evaluated based on how far the bird can travel without hitting obstacles.
3. **Selection:** The best-performing networks are selected to pass their genes to the next generation.
4. **Crossover and Mutation:** Selected networks undergo crossover and mutation to create a new generation of networks.
5. **Repeat:** The process repeats for a specified number of generations or until a network performs well enough.

## Results
As training progresses, you should observe improvements in the AI's performance. Initially, the birds will fail quickly, but over generations, they will learn to navigate the pipes more effectively.
