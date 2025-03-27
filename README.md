# Gradient Boosting on Digits Dataset

## Overview

This project implements and analyzes Gradient Boosting for handwritten digit classification using the scikit-learn `digits` dataset. It focuses on how **learning rate** and **number of estimators** affect model performance and overfitting.

## Dataset

- **Name**: Digits dataset (built-in from `sklearn.datasets`)
- **Samples**: 1797 images of digits (0–9)
- **Features**: 64 (8x8 pixel values)
- **Target**: Digit label (0–9)

## Workflow

1. **Data Exploration**
   - Checked shape, class distribution, and visualized digit samples
2. **Preprocessing**
   - No missing values; data ready for training
   - Split into train and test sets
3. **Model Training**
   - Used `GradientBoostingClassifier`
   - Trained over a grid of:
     - Learning rates (e.g., 0.01, 0.1, 0.5, 1.0)
     - Number of estimators (e.g., 50 to 250)
4. **Evaluation Metrics**
   - Accuracy scores (train/test)
   - Overfitting gap (difference between train and test accuracy)
   - Classification report
5. **Visualization**
   - Accuracy vs. estimators line plots



## Dependencies

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

## Conclusion

Gradient Boosting provides strong performance on digit classification. Tuning the learning rate and number of estimators is essential to prevent overfitting and maximize accuracy.
