# Cost-Sensitive Fraud Detection using Machine Learning

## Overview
This project implements a cost-sensitive fraud detection system that optimizes decision-making under real-world financial constraints.  
Instead of relying on accuracy or fixed thresholds, the model minimizes total expected business loss by balancing fraud detection against customer friction.

## Problem Motivation
In real banking systems:
- False negatives (missed fraud) cause direct financial loss
- False positives (blocked legitimate transactions) harm customer trust

Treating both errors equally leads to unrealistic decisions.  
This project addresses that gap using cost-aware optimization.

## Methodology
- Trained a Logistic Regression model to estimate fraud probabilities
- Applied feature scaling and handled class imbalance using class weighting
- Defined a realistic cost matrix for false positives and false negatives
- Optimized the decision threshold to minimize total expected cost

## Key Insight
The optimal decision threshold differed significantly from the default 0.5, demonstrating that real-world deployment requires cost-aware decision rules rather than metric-driven optimization.

## Technologies Used
- Python
- Scikit-learn
- NumPy, Pandas
- Matplotlib

## Results
- Produced probabilistic fraud risk scores
- Identified an optimal conservative threshold under high false-positive cost
- Demonstrated how business constraints influence ML decisions

## Future Work
- Categorical feature encoding
- Advanced ensemble models
- Model explainability using SHAP
- Evaluation under data drift

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/rajveersingharneja/cost-sensitive-fraud-detection.git
   cd cost-sensitive-fraud-detection
   
2. Install dependencies:
pip install -r requirements.txt

3. Launch the notebook:
   jupyter notebook notebooks/01_eda.ipynb
   
4. Run the notebook cells sequentially to reproduce the analysis and results.

## Author
Rajveer Arneja
