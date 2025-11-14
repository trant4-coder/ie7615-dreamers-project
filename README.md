# Explainable Deep Learning for Stress Prediction 

### Problem Definition

Mental health and wellness apps increasingly use AI to predict stress, mood, or anxiety from digital and lifestyle behaviors. While deep learning models can achieve strong predictive performance, they are often black boxes, leaving users and clinicians unable to understand why a certain prediction was made. This lack of transparency limits trust, adoption, and the safe use of AI-driven wellness tools.

Wellness app users, developers, and researchers need interpretable AI systems that can explain predictions of stress and well-being, because opaque “black box” models undermine trust, prevent accountability, and reduce actionable insights.

-------------------------
### Repository Structure

ie7516-dreamers-project/
- data/
  - Tech_Use_Stress_Wellness.csv
- notebook/
  - IE7615_Project_Dreamers.ipynb
- README.md

-------------------------
### How to Run the Code

#### Option 1 — Google Colab 
- Open the notebook in Colab:
- Upload the .ipynb file to Colab or
- Use "Open in Colab" if you add the badge
- Upload the dataset inside Colab
- Run each cell sequentially

#### Option 2 — Local machine
- Install all dependencies: pip install -r requirements.txt
- Run the notebook using Jupyter: jupyter notebook IE7615_Project_Dreamers.ipynb

-------------------------
### Dependencies
pandas, numpy 
scikit-learn
xgboost
lime 
shap
matplotlib, seaborn 

-------------------------
### Models Implemented

| Model               | Notes                           |
| ------------------- | ------------------------------- |
| Logistic Regression | Baseline linear model           |
| Decision Tree       | Simple tree classifier          |
| Random Forest       | Ensemble of trees               |
| XGBoost             | Best-performing classical model |
| MLP (baseline)      | Neural network with 2 layers    |
| MLP (deep/wide)     | Additional NN architectures     |

-------------------------
### Explainability Methods

#### LIME (Local Interpretable Model-Agnostic Explanations)

1. Used to explain individual predictions for:
- XGBoost
- MLP Neural Network

2. Displays:
- Feature contributions
- Prediction probabilities
- Comparison with true label

#### SHAP (SHapley Additive exPlanations)
1. Applied to:
- XGBoost
- MLP 

2. Shows:
- Global feature importance
- Direction and magnitude of effects
- Consistency of model reasoning
