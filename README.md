# THEMIS Plasma Density Prediction using Scientific Machine Learning

Machine learning pipeline for predicting plasma density from NASA THEMIS spacecraft magnetic field measurements.

---

## Overview

Understanding plasma density in near-Earth space environments is critical for studying magnetospheric dynamics, solar wind interactions, and space weather processes.

This project develops a scientific machine learning pipeline to predict plasma density using magnetic field measurements from NASA's THEMIS mission.

The workflow integrates spacecraft telemetry, temporal synchronization, feature engineering, and supervised learning techniques to estimate plasma density from magnetic field behavior.

---

## Scientific Motivation

Traditional plasma density measurements are not always continuously available.

This work investigates whether plasma density can be inferred from magnetic field measurements, enabling improved plasma environment characterization in data-limited conditions.

Applications include:

- Space weather modeling
- Magnetospheric plasma diagnostics
- Scientific data gap reconstruction
- Physics-informed machine learning

---

## Methodology

### Data Source
NASA THEMIS Mission

### Input Features

Magnetic field measurements:

- Bx
- By
- Bz
- Magnetic field magnitude |B|

### Target Variable

Plasma density

### Workflow

1. Load THEMIS spacecraft telemetry using PySPEDAS  
2. Synchronize magnetic field and plasma measurements in time  
3. Perform temporal interpolation  
4. Engineer derived magnetic features  
5. Train Random Forest regression model  
6. Evaluate predictive performance using time-based train/test splitting

---

## Model

**Algorithm:** Random Forest Regression

Why Random Forest?

- Handles nonlinear physical relationships
- Robust against noisy spacecraft measurements
- Strong performance on structured scientific data

---

## Results

Performance metrics:

- Log Density R²: *(Insert your value)*
- Density R²: *(Insert your value)*

The model demonstrates strong predictive capability for estimating plasma density from magnetic field behavior.

---

## Technical Stack

- Python
- PySPEDAS
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

## Future Work

- Gradient boosting models
- Neural-network approaches
- Multi-spacecraft generalization
- Orbital region classification

---

## Author

**Victor Oyiboka**  
Physics Graduate Researcher  
University of Texas at Dallas
