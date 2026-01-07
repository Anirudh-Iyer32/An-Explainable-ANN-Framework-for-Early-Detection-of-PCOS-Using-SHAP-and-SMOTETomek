# An-Explainable-ANN-Framework-for-Early-Detection-of-PCOS-Using-SHAP-and-SMOTETomek
Overview

Polycystic Ovary Syndrome (PCOS) is a common endocrine disorder affecting women of reproductive age. Early detection plays a crucial role in effective treatment and long-term health management.

This project implements a robust PCOS prediction system using an Artificial Neural Network (ANN), enhanced with advanced data preprocessing, class balancing techniques, multiple model iterations for generalization, and explainable AI (XAI) for interpretability.

Objectives

Predict PCOS using clinical and lifestyle features

Address class imbalance using advanced resampling techniques

Improve model generalization through multiple ANN architectures

Handle skewed data distributions during preprocessing

Provide transparent and interpretable predictions using XAI

Dataset Description

The dataset consists of medical and physiological attributes relevant to PCOS diagnosis, including:

Age

BMI

Hormonal indicators

Menstrual cycle characteristics

Clinical and lifestyle parameters

Technologies Used

Python

NumPy

Pandas

Matplotlib / Seaborn

Scikit-learn

TensorFlow / Keras

Imbalanced-learn

SHAP

Jupyter Notebook

Advanced Data Preprocessing
Skewness Treatment

Numerical features were analyzed for skewness

Logarithmic and power transformations were applied where necessary

Ensured more symmetric feature distributions for stable ANN training

Feature Scaling

Standardization or normalization applied after skewness treatment

Prevented dominance of high-magnitude features

Class Balancing Strategy
SMOTE-Tomek Resampling

Used a hybrid approach combining SMOTE and Tomek Links

SMOTE generated synthetic samples for the minority PCOS class

Tomek Links removed overlapping and noisy samples

Resulted in cleaner decision boundaries and improved class separability

This advanced balancing technique significantly improved model robustness compared to basic oversampling methods.

Model Architecture and Training
Artificial Neural Network (ANN)

Fully connected feedforward neural network

ReLU activation functions in hidden layers

Sigmoid activation in the output layer for binary classification

Binary Cross-Entropy loss function

Adam optimizer

Iterative Model Development

Multiple ANN architectures were trained with varying:

Number of hidden layers

Neurons per layer

Learning rates

Epoch counts

Performance compared across iterations to discover optimal generalization

Overfitting controlled using validation monitoring and regularization strategies

Model Evaluation Metrics

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

Evaluation focused on balanced performance with special emphasis on clinical relevance.

Explainable AI (XAI) Using SHAP

To ensure transparency and trust in predictions:

SHAP (SHapley Additive exPlanations) was used for model interpretability

Feature-level contribution analysis was performed

Global and local explanations were generated

Enabled understanding of how individual features influence PCOS predictions

This approach bridges the gap between black-box ANN models and real-world healthcare interpretability.

Results

Improved predictive stability after SMOTE-Tomek balancing

Better generalization observed across ANN iterations

Clear feature importance insights obtained using SHAP

Model suitable for healthcare decision-support systems

(Note: Exact performance metrics may vary based on data splits and training configurations.)

