Title: Traffic Accident Prediction using Machine Learning


This project aims to develop a Traffic Accident Prediction System that forecasts the likelihood of traffic accidents based on factors such as weather, time, road conditions, traffic density, and driver behavior. The objective is to assist traffic management authorities and emergency services in proactively reducing accidents and enhancing road safety.

Dataset: 
Source = https://www.kaggle.com/datasets/denkuznetz/traffic-accident-prediction/data

Size: 840 instances

Features: 14 (10 categorical, 4 quantitative)

Target Variable:

  *Accident: Binary classification (1 = Accident, 0 = No Accident)

Key Features:

| Feature              | Type         | Description                            |
| -------------------- | ------------ | -------------------------------------- |
| Weather              | Categorical  | Weather conditions                     |
| Road\_Type           | Categorical  | Type of the road                       |
| Time\_of\_day        | Categorical  | Time of day                            |
| Traffic\_Density     | Categorical  | Traffic density                        |
| Speed\_Limit         | Quantitative | Speed limit of the road                |
| Number\_Of\_Vehicles | Quantitative | Number of vehicles on the road         |
| Driver\_Alcohol      | Categorical  | Whether the driver is under alcohol    |
| Accident\_Severity   | Categorical  | Severity of the accident (if occurred) |
| Road\_Condition      | Categorical  | Road condition                         |
| Vehicle\_Type        | Categorical  | Type of vehicle                        |
| Driver\_Age          | Quantitative | Age of the driver                      |
| Driver\_Experience   | Quantitative | Years of driving experience            |
| Road\_Light          | Categorical  | Road lighting condition                |
| Accident (Target)    | Categorical  | Accident occurrence (1/0)              |


Data Preprocessing

*Missing Values:

1. Quantitative: Imputed using Median

2. Categorical: Imputed using Mode

*Categorical Encoding:

1. One-Hot Encoding applied to all categorical features (except binary Driver_Alcohol).

*Feature Scaling:

1. Used Robust Scaler on Speed_Limit, Number_Of_Vehicles, Driver_Age, and Driver_Experience to handle outliers.

*Dataset Split:

1. 70% Training

2. 30% Testing

