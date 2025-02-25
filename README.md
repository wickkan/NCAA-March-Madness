# March Machine Learning Mania 2025

## Overview
This repository contains code and data used to predict match outcomes for the NCAA March Madness 2025 men's and women's basketball tournaments. The project leverages advanced machine learning techniques and historical data to generate highly accurate predictions, optimized to minimize the Brier Score, the competition's official evaluation metric.

## Features
- **Enhanced ELO Ratings**: Computes dynamic ELO ratings for teams based on regular season performance, incorporating margin-of-victory and home-court advantage adjustments.
- **Advanced Team Statistics**: Derives detailed metrics (e.g., field goal percentages, rebounds, assists, turnovers) from regular season detailed results for robust feature engineering.
- **Hybrid Machine Learning Model**: Combines:
  - ELO-based probabilities for historical team strength.
  - XGBoost classifier trained on matchup-specific features for complex pattern recognition.
  - Probability calibration via Platt scaling for refined predictive accuracy.
- **Efficient Data Processing**: Includes memory optimization to handle large datasets efficiently on Kaggle.
- **Comprehensive Submission Generation**: Produces predictions for all possible 2025 tournament matchups using a calibrated ensemble approach.

## Model Performance
Validation was performed on the 2024 NCAA tournament games as a holdout set. The Brier scores reflect the model's performance after ELO computation, XGBoost training, and calibration:

| Model         | Brier Score |
|---------------|-------------|
| Men's Model   | 0.0060      |
| Women's Model | 0.0065      |
| Average       | 0.0062      |

**Note**: These scores are exceptionally low, suggesting either an extraordinarily effective model or potential data leakage (e.g., 2024 games included in training). Further validation on additional years (e.g., 2023) is recommended to confirm generalizability.

## Potential Improvements
- **Data Leakage Check**:
  - Ensure training data excludes 2024 to validate true predictive power on unseen data.
- **Feature Engineering**:
  - Integrate external rankings (e.g., Massey Ordinals) for additional context.
  - Add player-level statistics or injury data if available.
  - Explore pace-adjusted metrics to refine efficiency calculations.
- **Model Optimisation**:
  - Experiment with hyperparameter tuning for XGBoost (e.g., learning rate, max depth).
  - Test ensemble weighting variations (e.g., 0.8 ELO, 0.2 XGBoost) for optimal blending.
  - Incorporate neural networks or gradient boosting alternatives for comparison.
- **Simulation Approach**:
  - Implement Monte Carlo simulations to model tournament bracket variability.
  - Adjust probabilities for seed-based upsets or late-round dynamics.
- **Cross-Validation**:
  - Validate across multiple past tournaments (e.g., 2020–2023) to assess robustness.

## References & Acknowledgements
- **Kaggle Competition**: [March Machine Learning Mania 2025](https://www.kaggle.com/c/march-machine-learning-mania-2025)
- **Inspiration**: Techniques inspired by top solutions from the 2024 competition, including ensemble modeling and calibration.

## Collaborators
- [wickkan](https://github.com/wickkan)
- [stephendwalley](https://github.com/stephendwalley)

## License
This project is licensed under the MIT License
