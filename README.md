# APCV 485 Coding Lab 2

## Network Traffic Anomaly Detection

This lab builds an anomaly-detection pipeline for cybersecurity traffic analysis using the NSL-KDD dataset and an autoencoder-based approach.

## What this lab covers

- Preprocessing mixed network-traffic features
- Training an autoencoder to learn normal behavior
- Detecting anomalies from reconstruction error
- Evaluating with accuracy, precision, recall, F1, ROC/AUC, and confusion matrix
- Exploring threshold strategies and bonus model ideas

## Results snapshot

Baseline run in the notebook reports approximately:

- Accuracy: **0.815**
- Precision: **0.957**
- Recall: **0.707**
- F1 Score: **0.813**

These results highlight a strong precision profile and a clear precision-recall tradeoff controlled by threshold choice.

## Artifacts generated

- `roc_curve.png`
- `confusion_matrix.png`
- `training_history.png`
- `error_distribution.png`

## Files

- `network-traffic-anomaly-detection.ipynb` - full training, detection, and analysis workflow

## How to run

1. Open the notebook in Jupyter or Google Colab.
2. Ensure dataset files are available (for example, NSL-KDD train/test files used by the notebook).
3. Install dependencies if needed:
   - `tensorflow`
   - `numpy`
   - `pandas`
   - `matplotlib`
   - `scikit-learn`
4. Run all cells top to bottom.

## Why this is cool

Instead of only classifying known patterns, this workflow learns what "normal" looks like and flags unusual behavior. That makes it a practical baseline for real-world cyber monitoring where new attack variants can appear over time.
