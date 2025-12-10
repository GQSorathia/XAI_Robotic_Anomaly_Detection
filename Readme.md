# Explainable AI for Robotic Anomaly Detection

## Overview
Multi-class anomaly detection system for robotic telemetry data that distinguishes between Normal Operation, DoS Attack, and Malfunction using machine learning models with explainability techniques.

## Dataset
- **Features**: 52 numerical features (position, orientation, velocity, IMU, RSSI, battery)
- **Classes**: Normal, DoS_Attack, Malfunction
- **Samples**: ~50,000 records

## Explainability Techniques
- Permutation Importance
- SHAP (SHapley Additive exPlanations)
- LIME (Local Interpretable Model-agnostic Explanations)
- Partial Dependence Plots
- Feature-Target Correlation Analysis

## Installation

### Google Colab
```python
!pip install shap lime xgboost lightgbm imbalanced-learn

```

## Expected Runtime

### With GPU (Google Colab)
- Data Preprocessing: 3-5 minutes
- Model Training: 20-30 minutes
- Model Evaluation:  3-5 minutes
- XAI Analysis: 15-20 minutes
- Model Saving: 1-2 minutes
- **Total: 45-65 minutes**

### Without GPU (CPU Only)
- Data Preprocessing: 5-8 minutes
- Model Training: 40-60 minutes
- Model Evaluation: 5-8 minutes
- XAI Analysis: 20-30 minutes
- Model Saving: 2-3 minutes
- **Total: 70-110 minutes**

## Running the Code

### Step-by-Step Execution

1. **Upload notebook** to Google Colab
2. **Enable GPU**: Runtime → Change runtime type → Hardware accelerator → GPU
3. **Install dependencies** (see Installation section above)
4. **Run cells sequentially**: 
   - Part 1: Data Preprocessing
   - Part 2: Model Training
   - Part 3: Model Evaluation
   - Part 4: XAI Analysis
   - Part 5: Save Models
