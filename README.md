This repository explores hybrid volatility forecasting models that combine traditional GARCH(1,1) dynamics with deep learning architectures in PyTorch.
The goal is to evaluate how much predictive performance can be improved by adding neural-network components on top of classical econometric models.



Project Overview
We benchmark three approaches:


GARCHNN (Frozen Features)

A neural network that predicts GARCH-like volatility parameters
Feature extractor is not fine-tuned
Trained only on the parameter head


GARCHNN (Fine-Tuned)
Same architecture, but the feature extractor is fully trainable
Evaluates whether end-to-end training improves forecasting accuracy


Classical GARCH Baseline
GARCH(1,1) model implemented with PyTorch / GARCH libraries
Serves as a reference for how well traditional models perform on synthetic time series



Objectives
Compare volatility forecasting performance across all models

