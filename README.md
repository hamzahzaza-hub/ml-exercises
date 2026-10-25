# Hands-On Machine Learning – My Exercises

My notebooks and exercise solutions while working through
*Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* (3rd edition)
by Aurélien Géron.

I added my own comments to the code to explain what each step does and why.

## Chapters

## What I learned in Chapter 2
- Loading and exploring data with pandas
- Making a stratified train/test split
- Cleaning data: filling missing values, one-hot encoding, scaling
- Building preprocessing pipelines with scikit-learn
- Training and comparing models (Linear Regression, Decision Tree, Random Forest, SVR)
- Tuning hyperparameters with GridSearchCV and RandomizedSearchCV
- Final result: Random Forest with about $41,000 RMSE on the test set

## What I learned in Chapter 3
- Building an image classifier for handwritten digits (MNIST) with K-Nearest Neighbors
- Tuning `n_neighbors` and `weights` with grid search to reach **97%+ accuracy**
- Data augmentation: shifting images by 1 pixel to grow the training set (about 17% fewer errors)
- Predicting Titanic survival: SVM (~82.5%) vs. Random Forest (~81.4%) with cross-validation
- Building a spam filter: turning emails into word-count vectors (lowercase, URLs, numbers, stemming)
- Measuring classifiers with precision and recall, not just accuracy

## What I learned in Chapter 4
- How Linear Regression is trained: the Normal Equation vs. Gradient Descent
- Batch, Stochastic, and Mini-batch Gradient Descent, and when to use each one
- Why feature scaling matters for Gradient Descent
- Spotting overfitting vs. underfitting with learning curves
- Regularization: Ridge (ℓ₂), Lasso (ℓ₁), and Elastic Net
- Early stopping: keep the best model and use "patience" instead of stopping at the first bad epoch
- Logistic Regression and Softmax Regression for classification
- Built Softmax Regression **from scratch with only NumPy** (Batch GD + ℓ₂ + early stopping) on the iris dataset: **96.7% test accuracy**

## How to run
1. Install Python 3.10 or newer
2. Install the libraries:
   pip install numpy pandas matplotlib scikit-learn scipy jupyter nltk urlextract
3. Open a notebook in VS Code or Jupyter and click **Run All**

Note: some cells (grid search, KNN on MNIST) take several minutes to run.

