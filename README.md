# Neural-Network-Generalization-Reliability-Healthcare-Risk-Prediction
Neural network-based healthcare risk classification project analyzing model generalization, overfitting, regularization, and prediction reliability using MLP models
## Project Overview
This project investigates the generalization ability and reliability of neural networks for healthcare risk prediction. A Multilayer Perceptron (MLP) model was developed to classify individuals into four health-risk tiers using physiological and behavioral indicators.

The study goes beyond achieving high predictive accuracy by evaluating model generalization, identifying overfitting, assessing prediction reliability, and comparing the performance of a baseline neural network against a dropout-regularized model.

---

## Objectives

- Develop a baseline neural network for healthcare risk classification.
- Evaluate model generalization performance.
- Identify overfitting using learning curves.
- Improve model performance through dropout regularization.
- Analyze prediction errors using confusion matrices.
- Assess prediction confidence and model reliability.

---

## Dataset

The project uses a healthcare risk dataset containing:

- **1,500 observations**
- **18 predictive features**
- **4 health-risk categories (Tier 0 – Tier 3)**

The features represent physiological and behavioral indicators used to predict an individual's health-risk level.

---

## Tools & Technologies

- Python
- Jupyter Notebook
- TensorFlow / Keras
- Scikit-learn
- NumPy
- Pandas
- Matplotlib

---

## Methodology

### Data Preparation

- Missing value analysis
- Stratified Train / Validation / Test split
- Feature standardization using StandardScaler
- Class distribution analysis

### Neural Network Models

### Baseline Model

- Dense (64 neurons, ReLU)
- Dense (32 neurons, ReLU)
- Softmax Output Layer

### Regularized Model

The second model introduced:

- Dropout (0.4)
- Same hidden layer architecture
- Softmax output layer

This allowed a fair comparison between the baseline and regularized neural networks.

---

## Model Evaluation

The models were evaluated using:

- Accuracy
- Macro Precision
- Macro Recall
- Macro F1-Score
- Confusion Matrix
- Learning Curves
- Confidence Analysis

Macro-averaged metrics were prioritized due to class imbalance and the importance of correctly identifying high-risk patients.

---

## Results

### Baseline Model

- Strong overfitting observed
- High training accuracy
- Validation performance plateaued
- Large training-validation performance gap

### Dropout-Regularized Model

Performance improved significantly through dropout regularization.

| Metric | Score |
|---------|------:|
| Accuracy | **0.747** |
| Macro Precision | **0.709** |
| Macro Recall | **0.699** |
| Macro F1-Score | **0.703** |

The regularized model demonstrated improved generalization and produced more reliable predictions compared to the baseline model.

---

## Key Findings

- Dropout effectively reduced overfitting.
- Generalization improved substantially.
- Most prediction errors occurred between adjacent health-risk tiers.
- High-confidence predictions were generally more accurate.
- Prediction reliability increased with confidence scores.

---

## Repository Structure

```
Neural-Network-Generalization-Reliability-Healthcare-Risk-Prediction
│
├── notebooks/
│   └── Neural_Network_Generalization_Reliability.ipynb
│
├── report/
│   └── Neural_Network_Generalization_Reliability_Report.pdf
│
├── images/
│   ├── baseline_learning_curve.png
│   ├── dropout_learning_curve.png
│   ├── confusion_matrix.png
│   └── confidence_analysis.png
│
├── requirements.txt
│
└── README.md
```

---

## Skills Demonstrated

- Machine Learning
- Deep Learning
- Neural Networks
- TensorFlow / Keras
- Data Preprocessing
- Model Evaluation
- Regularization Techniques
- Classification
- Performance Metrics
- Data Visualization
- Healthcare Analytics

---

## Future Improvements

Potential enhancements include:

- Class-weighted loss functions
- Probability calibration (Temperature Scaling)
- Early stopping
- L2 regularization
- Hyperparameter optimization
- Larger and more balanced datasets

---

## Project Highlights

✔ Developed two neural network architectures for comparison.

✔ Evaluated model generalization using training and validation learning curves.

✔ Applied dropout regularization to improve predictive performance.

✔ Performed confusion matrix and error analysis to understand model behavior.

✔ Assessed prediction confidence to evaluate model reliability.

---

## Disclaimer

This project was completed as part of the Master of Data Analytics program and is shared for educational and portfolio purposes. The analysis, implementation, evaluation, and interpretation presented in this repository reflect my work and are intended to demonstrate practical machine learning and deep learning skills.
