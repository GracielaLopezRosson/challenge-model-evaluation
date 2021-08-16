# Model evaluation challenge - US Income

# Description
The mission is *to predict the income of every US citizen*, using `RandomForestClassifier()` from `sklearn`.   

## Mission objectives

- Be able to analyze a machine learning problem
- Be able to reason about possible causes of overfitting
- Be able to remedy the causes of overfitting
- Be able to tune parameters of a machine learning model
- Be able to write clean and documented code.

# Installation

## Python version
* Python 3.9


## Packages used
* pandas
* numpy
* matplotlib.pyplot
* seaborn
* sklearn

# Usage
| File                | Description                                                    |
|---------------------|----------------------------------------------------------------|
| cleaned_dataset.csv | Original dataset acquired by Immo Eliza                        |
| df2_regions.csv     | Output of Clean.py  <br>Cleaned data to use in the Machine-Learning-model |
| Regression.py       | File containing Python code  <br>This file was used to:  <br>1. split Belgium between regions:    <br>* Wallonia  <br>* Flanders  <br>* Brussels <br>2. Make a Machine-Learning-model for every region<br> |
| Clean.py            | File containing Python code  <br>This file was used to clean the database (cleaned_dataset.csv) |


# Results

Features of the dataset: 
[age, workclass, fnlwgt education, education-num, marital-status, occupation, relationship, race, sex, capital-gain, capital-loss, hours-per-week, native-country]	


## Data visualization
**Heatmap showing some correlations bettween the features on the dataset.**

![](visuals/heatmap.png)

**Income related to age**

![](visuals/income_age.png)

**Income related to gender**

![](visuals/income_sex.png)
We can see here that there is still a huge gap in income between male and female.

**Income related to race**

![](visuals/income_race.png)
From here we notice that mainly white people have income >50k.

## Baseline

Using the dataset (data_train.csv) as it is (after checking for NaNs and dropping duplicates), splitting it in 75% training and 25% test, the metrics obtained are:


| Metrics                 | Score          |
|-----------------------|------------------|
| accuracy	| 0.86            |
|roc_auc_score	| 0.90            |
|matthews_corrcoef | 0.60            |
|MAE		| 0.14            |
|MQE		| 0.14            |
|R2		| 0.23            |
|Cross validation|            |


**Classification report**
![](visuals/class_report.png)

**Confusion matrix**
![](visuals/confusion_matrix.png)

**ROC curve**
![](visuals/roc.png)

# Contributors
| Name                  | Github                                 |
|-----------------------|----------------------------------------|
| Graciela Lopez Rosson | https://github.com/GracielaLopezRosson |
         




# Timeline
16-08-2021
