# March Machine Learning Mania 2025

## Overview
This repository contains code and data used to predict match outcomes for the NCAA March Madness 2025 men's and women's basketball tournaments. The project is designed to optimize predictions based on historical team performance and tournament data while minimizing the Brier Score, the competition's official evaluation metric.

## Features
- **Team-Level Statistics Computation**: Calculates win ratio, average points scored, points allowed, and point margins from regular season data.
- **Feature Engineering**: Computes matchup-specific differences in team statistics to predict outcomes.
- **Machine Learning Model**: Uses logistic regression to classify matchups with probabilities.
- **Efficient Data Processing**: Optimized memory handling to run on Kaggle without crashes.
- **Automated Tournament Simulation**: Generates possible matchups for 2025 and predicts outcomes.

## Model Performance
| Model | Brier Score |
|--------|------------|
| Men's Model | 0.2249 |
| Women's Model | 0.2612 |

## Potential Improvements
- **Feature Engineering**:
  - Incorporate advanced statistics such as offensive and defensive efficiencies.
  - Include historical ELO rankings and other ranking systems.
  - Consider impact of home-court advantage.
- **Model Optimization**:
  - Try more advanced models like XGBoost, Random Forests, or Neural Networks.
  - Tune hyperparameters using grid search.
- **Simulation Approach**:
  - Implement Monte Carlo simulation for better tournament outcome predictions.
  - Adjust probabilities dynamically based on seeding and round progression.

## References & Acknowledgements
- **Kaggle Competition**: [March Machine Learning Mania 2025](https://www.kaggle.com/c/march-machine-learning-mania-2025)

## Collaborators
- [wickkan](https://github.com/wickkan)
- [stephendwalley](https://github.com/stephendwalley)

## License
This project is licensed under the MIT License
