# Hands-On Machine Learning – My Exercises

My notebooks and exercise solutions while working through
*Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* (3rd edition)
by Aurélien Géron.

I added my own comments to the code to explain what each step does and why.

## Chapters

| Chapter | Topic | Files |
|---|---|---|
| 2 | End-to-end ML project: predicting California house prices | [Notebook](chapter-02-housing/02_end_to_end_machine_learning_project.ipynb), [Exercises](chapter-02-housing/02_exercises.ipynb) |
| 3 | Classification: MNIST digits, Titanic, spam filter | [Exercises](chapter-03-classification/03_exercises.ipynb) |

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

## How to run
1. Install Python 3.10 or newer
2. Install the libraries:
   pip install numpy pandas matplotlib scikit-learn scipy jupyter nltk urlextract
3. Open a notebook in VS Code or Jupyter and click **Run All**

Note: some cells (grid search, KNN on MNIST) take several minutes to run.

## Credit
Based on the book and the official notebooks:
https://github.com/ageron/handson-ml3 (Apache 2.0 license)
