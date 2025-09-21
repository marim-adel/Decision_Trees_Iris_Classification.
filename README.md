🌸 Iris Classification with Decision Tree
📌 Overview

This project applies a Decision Tree Classifier to the classic Iris dataset (150 samples, 4 features, 3 classes).
The goal is to explore the dataset, preprocess it, train a decision tree, and evaluate classification performance.

📊 Dataset & EDA

Dataset: Iris Dataset

Features:

Sepal Length

Sepal Width

Petal Length

Petal Width

Target classes:

Setosa

Versicolor

Virginica

Exploratory Data Analysis (EDA)

✔ Checked missing values → none found.
✔ Removed duplicate rows → 1 duplicate removed.
✔ Plotted pairplots and correlations for feature relationships.

⚙️ Preprocessing

Dropped duplicates from df.

Scaled features using StandardScaler.

Train-test split: 80/20 with stratified sampling.

🌳 Model Training

Algorithm: Decision Tree Classifier

Parameters:

max_depth=2 (controlled complexity to avoid overfitting)

random_state=42 (reproducibility)

Trained on scaled features X_train, y_train.

📈 Evaluation
Metrics
Accuracy: 0.67
F1 Score: 0.56

Classification Report:
              precision    recall  f1-score   support

      setosa       1.00      1.00      1.00        15
  versicolor       0.50      1.00      0.67        15
   virginica       0.00      0.00      0.00        15

🔎 Summary

Setosa: Perfectly classified ✅

Versicolor: High recall (1.0) but precision suffers (0.5)

Virginica: Not correctly classified ❌

Overall Accuracy: ~67% → indicates underfitting due to shallow tree.

🚀 Next Steps

To improve accuracy toward 95%+:

Increase max_depth or tune min_samples_split / min_samples_leaf.

Try Random Forest or Gradient Boosting.

Use cross-validation to better estimate generalization.

Visualize tree structure for interpretability.active predictions.
