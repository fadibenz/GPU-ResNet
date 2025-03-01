# GPU Memory Considerations in Neural Network Training

## Overview

This notebook explores the impact of GPU memory usage when training neural networks, specifically focusing on the ResNet model trained on the CIFAR-10 dataset using PyTorch. The notebook investigates various system considerations, including the effect of batch size on memory usage, the impact of different optimizers (SGD, SGD with momentum, Adam), and techniques to minimize memory usage through gradient accumulation.

## Key Topics Covered

1. **Environment Setup**: Setting up the necessary environment for training neural networks on GPUs.
2. **Dataset Preparation**: Downloading and preprocessing the CIFAR-10 dataset.
3. **Model Analysis**: Analyzing the memory usage of the ResNet-152 model and CIFAR-10 input sizes.
4. **GPU Memory Utilization**: Using `nvidia-smi` to measure GPU memory utilization.
5. **Optimizer Memory Usage**: Comparing the memory usage of different optimizers (SGD, SGD with momentum, Adam).
6. **Batch Size Impact**: Investigating the effect of batch size on convergence and GPU memory usage.
7. **Gradient Accumulation**: Techniques to minimize memory usage during training.

## Starter Code

The starter code for this notebook is provided by CS182. The code includes helper functions for memory profiling, training, and testing the model, as well as utilities for logging memory usage and analyzing model performance.

## Usage

1. **Setup**: Ensure that the environment is set up with the necessary libraries and dependencies. The notebook assumes the use of a GPU for training.
2. **Dataset**: The CIFAR-10 dataset is automatically downloaded and preprocessed.
3. **Training**: The notebook includes functions to train the ResNet model with different optimizers and batch sizes. Memory usage is logged and analyzed throughout the training process.
4. **Analysis**: The notebook provides visualizations and insights into the memory usage patterns and performance of the model under different configurations.

## Dependencies

- Python 3.x
- PyTorch
- torchvision
- numpy
- matplotlib
- pandas
- GPUtil

## Running the Notebook

1. **Install Dependencies**: Ensure all required libraries are installed.
   ```bash
   pip install torch torchvision numpy matplotlib pandas GPUtil
   ```
2. **Run the Notebook**: Open the notebook in a Jupyter environment and execute the cells sequentially. The notebook includes detailed comments and instructions for each step.
