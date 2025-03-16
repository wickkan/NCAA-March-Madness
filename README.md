# March Machine Learning Mania 2025

## Overview
This repository contains code and data used to predict match outcomes for the NCAA March Madness 2025 men's and women's basketball tournaments. The project leverages advanced machine learning techniques and historical data to generate highly accurate predictions, optimised to minimise the Brier Score, the competition's official evaluation metric.

## Features
- **Enhanced ELO Ratings**: Computes dynamic ELO ratings for teams based on regular season performance, incorporating margin-of-victory and home-court advantage adjustments.
- **Advanced Team Statistics**: Derives detailed metrics (e.g., field goal percentages, rebounds, assists, turnovers) from regular season detailed results for robust feature engineering.
- **Hybrid Machine Learning Model**: Combines:
  - ELO-based probabilities for historical team strength.
  - XGBoost classifier trained on matchup-specific features for complex pattern recognition.
  - Probability calibration via Platt scaling for refined predictive accuracy.
- **Efficient Data Processing**: Includes memory optimisation to handle large datasets efficiently on Kaggle.
- **Comprehensive Submission Generation**: Produces predictions for all possible 2025 tournament matchups using a calibrated ensemble approach.

## References & Acknowledgements
- **Kaggle Competition**: [March Machine Learning Mania 2025](https://www.kaggle.com/c/march-machine-learning-mania-2025)

## Collaborators
- [wickkan](https://github.com/wickkan)
- [stephendwalley](https://github.com/stephendwalley)

## License
This project is licensed under the MIT License
