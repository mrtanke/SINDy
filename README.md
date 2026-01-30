## SINDy: Sparse Identification of Nonlinear Dynamics

Implementation of the SINDy algorithm for discovering governing equations from data, applied to pendulum dynamics.

![Overview of SINDy Autoencoder](/SINDy-Autoencoder.jpeg)

### Overview

This project implements symbolic regression using SINDy to identify the pendulum equation $\ddot{z} = -\sin(z)$ from simulated data. It includes:

- **Basic SINDy**: LASSO regression with sklearn and PyTorch implementations
- **Thresholding Algorithms**: Sequential Thresholding (ST) and Patient Trend-Aware Thresholding (PTAT)
- **SINDy-Autoencoder**: Learning dynamics from Cartesian coordinates and video data
- **Derivative Propagation**: Custom neural network layers for time derivative computation

### Usage

Open and run `sindy.ipynb` in Jupyter:

```bash
jupyter notebook sindy.ipynb
```

Execute cells sequentially to:
1. Simulate pendulum dynamics
2. Train SINDy models with different thresholding methods
3. Build and train SINDy-Autoencoders
4. Evaluate learned equations and visualize results
