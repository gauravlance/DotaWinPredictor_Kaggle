# Dota 2 Match Outcome Prediction (Kaggle)

This project is a machine learning approach to predicting the outcome of Dota 2 matches using features from a Kaggle-provided dataset. It was developed as part of a competition-style workflow, with a final submission evaluated via AUC score.

---

## Dataset

The dataset was provided by Kaggle and includes:
- `train_features.csv`: Match-level statistics
- `train_targets.csv`: Labels indicating whether the Radiant side won (`1`) or lost (`0`)
- `test_features.csv`: For final prediction and submission

> Note: The dataset is not included in this repository due to Kaggle’s data-sharing policy. The dataset can be obtained from https://www.kaggle.com/competitions/mlcourse-dota2-win-prediction/data

---

## Model Pipeline

The modeling process includes:
- Data preprocessing (handling missing values, encoding)
- Feature selection & basic exploration
- Model training using:
  - Logistic Regression (final model)
  - Random Forest
  - XGBoost (tested but not used for submission)
- Evaluation using **ROC AUC Score**

---

## Results

- Final validation AUC: **0.821** using Logistic Regression
- Kaggle leaderboard rank: **540th**



##  How to Run

1. Clone this repo
2. Download the dataset from Kaggle and place it under a `data/` directory
3. Run the notebook:  
   ```bash
   jupyter notebook DotaBaselinePredictionKaggleDataset.ipynb
   ```


---

## 🔍 Future Improvements

- Try feature engineering on hero picks
- Tune hyperparameters or try ensemble models
- Incorporate game time-series data if available

---

## 📌 Notes

- This was developed as part of a personal learning project and Kaggle competition.
- If you're interested in esports analytics or ML with tabular data, feel free to fork or reuse the code!# DotaWinPredictor_Kaggle
Dota Win prediction model I made using 3 models for a kaggle competition. Dataset analysed using logistic regression, random forests and XGboost
