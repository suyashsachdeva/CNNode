# CNNode: Neural ODE Testing on Circuit Components Dataset

This repository contains an implementation of Neural Ordinary Differential Equations (Neural ODEs) applied to a circuit components dataset. Neural ODEs differ from standard neural networks by incorporating the concept of continuous time dynamics, modeled through differential equations. This allows them to capture the rate of change in the data, making them particularly well-suited for applications where learning temporal or dynamic behavior is critical.

## Key Concepts

- **Standard Neural Networks (NNs):** Traditional neural networks model data as a direct transformation: `x = f(x)`, where `f` is a learned function that maps input to output.
- **Neural ODEs:** In contrast, Neural ODEs define the relationship through a differential equation: `dx/dt = f(x, t)`, where the model learns the rate of change over time. This makes Neural ODEs effective at learning dynamic systems.

## About the Repository

In this repository, we train and test a Neural ODE model on a dataset of circuit components, comparing its performance with a standard neural network. The objective is to evaluate how well Neural ODEs capture the dynamic nature of the data, compared to traditional neural networks.

## Results

- **Accuracy of Neural ODE (NODE):** 98%
- **Accuracy of Standard Neural Network (NN):** 97.4%

The results demonstrate that Neural ODEs slightly outperform standard NNs on this dataset, particularly in capturing dynamic relationships between features.

## Requirements

- Python 3.9
- PyTorch
- torchdyn (ODE Solver)
- numpy
- matplotlib
- OpenCV

