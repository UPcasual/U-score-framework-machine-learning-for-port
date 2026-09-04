# Decision-Horizon-Aware Machine Learning for Port Operational-Time Prediction

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Overview

This repository contains the implementation of a **decision-horizon-aware machine learning framework** for predicting port operational times. The framework evaluates models across three temporal horizons:

- **Ex Ante** (E-02): Predictions using only information available before vessel arrival
- **Intraoperational**: Predictions during vessel operations
- **Ex Post**: Full information predictions for benchmarking

## 🎯 Key Features

- **Multi-model ensemble**: Ridge, Random Forest, Extra Trees, XGBoost, LightGBM, CatBoost
- **Temporal horizon evaluation**: 3 distinct prediction scenarios
- **Comprehensive metrics**: U-metric (Performance × Interpretability × Actionability)^(1/3)
- **Feature importance**: SHAP analysis with stability testing
- **Counterfactual analysis**: Multi-observation scenario evaluation
- **Data leakage auditing**: Temporal consistency verification

## 📊 Results Summary

| Port | Horizon | Best Model | R² | MAE (h) | U-Metric |
|------|---------|------------|----|---------|----------|
| San Antonio | Ex Ante | LightGBM | 0.XXX | X.X | X.XXX |
| San Antonio | Intra | XGBoost | 0.XXX | X.X | X.XXX |
| San Antonio | Ex Post | CatBoost | 0.XXX | X.X | X.XXX |
| Coquimbo | Ex Ante | RandomForest | 0.XXX | X.X | X.XXX |
| Coquimbo | Intra | LightGBM | 0.XXX | X.X | X.XXX |
| Coquimbo | Ex Post | XGBoost | 0.XXX | X.X | X.XXX |

## 🚀 Quick Start

### Installation

```bash
git clone https://github.com/yourusername/Decision-Horizon-Aware-ML-Port-Time-Prediction.git
cd Decision-Horizon-Aware-ML-Port-Time-Prediction
pip install -r requirements.txt
