# Adaptive Traffic Signal Control Using Deep Q-Learning for Optimizing Traffic Clearance Times

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.16837904.svg)]([https://doi.org/10.5281/zenodo.16837904](https://doi.org/10.5281/zenodo.16837904))

## Overview
This project presents an **adaptive traffic signal control framework** using **Deep Q-Learning (DQL)** to optimize lane-by-lane clearance times at urban intersections. Unlike traditional fixed-phase systems, our agent predicts **continuous green times** for each lane, enabling fine-grained, real-time adjustments.

The system is trained in a **custom-built simulation** that incorporates:
- Traffic density and vehicle types
- Weather conditions
- Road conditions
- Time-of-day variations
- Random traffic incidents

## Key Features
- **Continuous Action Space**: Predicts optimal clearance time in seconds.
- **Dynamic Environment**: Realistic simulation with multiple traffic and environmental factors.
- **Deep Neural Network Agent**: Learns complex mappings from traffic states to optimal timings.
- **Experience Replay**: Stabilizes learning by randomizing past experiences.
- **Custom Reward Function**: Encourages precise time predictions.

## Methodology
1. **State Space**: 9 traffic and environmental features (vehicle counts, lanes, weather, road quality, etc.)
2. **Optimal Time Calculation**: Deterministic formula considering traffic volume and conditions.
3. **Model Architecture**: Two hidden layers (64 & 128 neurons, ReLU activation) with a linear output layer.
4. **Training Process**: Experience Replay and guided exploration strategy.

## Results
- Learned strategies closely approximate theoretical optima.
- Improved traffic throughput and reduced delays in simulation.
- Potential for deployment in **Intelligent Transportation Systems (ITS)**.

## Future Work
- Refined exploration strategies.
- Hyperparameter and reward tuning.
- Multi-agent coordination for network-wide optimization.

## Resources
- **Zenodo record**: [https://doi.org/10.5281/zenodo.16837904](https://doi.org/10.5281/zenodo.16837904)
- **Kaggle Notebook** (code & data): [Deep Q-Learning for AI Traffic Management System](https://www.kaggle.com/code/danishyousuf19/deep-q-learning-for-ai-traffic-management-system/notebook)

## Citation
If you use this work, please cite:

```D. Yousuf, “Adaptive Traffic Signal Control Using Deep Q-Learning for Optimizing Traffic Clearance Times”. Zenodo, Aug. 13, 2025. doi: 10.5281/zenodo.16837904.```
