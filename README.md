# Cardiac-Pathology-Prediction
It's is a challenge about Cardiac Pathology Prediction. It a 5-class classification problem and it is evaluated in this Kaggle website: https://www.kaggle.com/competitions/ima205-challenge-2023/overview

The project focuses on four heart conditions that may go initially unremarkable, but can eventually be life-threatening. Complications may include
severe heart failure and sudden cardiac arrest. More particularly, the aim is to classify MRI images of the heart into five diagnostic classes:
• ‘0’ Healthy controls

• ‘1’ Myocardial infarction

• ‘2’ Dilated cardiomyopathy

• ‘3’ Hypertrophic cardiomyopathy

• ‘4’ Abnormal right ventricle

Some of the relevant features help identify the state of the subject as the volume of the
different components of the cardiac system (Left Ventricle Cavity, Right Ventricle Cavity, and
Myocardium) at end diastle and at end systole, the Thickness of the Myocardium and the Ejection
Fractions of both of the left and right ventricle cavities. A segmentation part was needed to extract the region of interest.

![sss](https://github.com/souheib1/Cardiac-Pathology-Prediction/assets/73786465/90841386-68e0-453b-9442-1cb4d887a0fd)

![…](https://github.com/souheib1/Cardiac-Pathology-Prediction/assets/73786465/d2d80c8b-b9ee-44ae-98ad-01edd2c51f50)

## Evaluation of the Methods

| Model          | Validation Score | Accuracy on private leaderboard (Kaggle) | Optimal hyperparameters                       |
|:---------------|-----------------:|-----------------------------------------:|:---------------------------------------------|
| Decision Trees |           0.7875 |                                   0.6571 | min samples leaf: 2, criterion: gini          |
| Random Forest  |           0.8625 |                                   0.8    | n estimators: 30, max features: 'sqrt',      |
|                |                  |                                        | min_samples_leaf: 4, criterion: entropy      |
| KNN            |           0.85   |                                   0.7142 | K=7                                          |
| SVC            |           0.87   |                                   0.8    | kernel: linear, gamma: 0.01, C: 10           |
| MLP            |           0.864  |                                   0.8285 | solver: lbfgs, random state: 0,              |
|                |                  |                                        | hidden layer sizes: 250, alpha: 0.01        |






