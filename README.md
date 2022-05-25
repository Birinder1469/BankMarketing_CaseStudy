# Bank Marketing Case Study


## Problem statement 

The data set from UC Irvine’s Machine Learning Repository [Dataset url](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) includes direct marketing campaigns (i.e. phone calls) of a Portuguese banking institution. The goal is to predict if the client will subscribe a term deposit (indicated in the y variable). 


## Dataset

There are four datasets:

1. `bank-additional-full.csv` with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]<br>
2. `bank-additional.csv` with 10% of the examples (4119), randomly selected from 1), and 20 inputs.<br>
3. `bank-full.csv` with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs). <br>
4. `bank.csv` with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs).<br>

The smallest datasets are provided to test more computationally demanding machine learning algorithms (e.g., SVM). The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).

For this analysis I have used Dataset 1(bank-additional-full.csv) which is most recent and comprehensive.






## Analysis notebooks 

The processing was done in Google colab notebooks. The package versions are listed in the requirements.txt file.

Three notebooks listed below contain end to end implentation. 


[1 EDA.ipynb](https://github.com/Birinder1469/BankMarketing_CaseStudy/blob/main/1_EDA.ipynb)

Detailed exploratory data analysis. 

[2 Modelling.ipynb](https://github.com/Birinder1469/BankMarketing_CaseStudy/blob/main/2_Modelling.ipynb)

Data preparation and baseline model implemtation.

[3 ModelTuning HoldOut Dataset Evaluation.ipynb](https://github.com/Birinder1469/BankMarketing_CaseStudy/blob/main/3_ModelTuning_HoldOutDatasetEvaluation.ipynb)

Hyperparameter tuning and implementation of final model on the hold out dataset.



## Results 


| model|Train ROC-AUC score	 |Validation ROC-AUC score |Test ROC-AUC score |
| ------| ------	 | ------ | ------|
| Logistic Regression| 0.798736	 | 0.787251 | 0.789623|
| Random Forest| 0.802594	 | 0.787835 | 0.787706|
| XGBoost | 0.825193	 | 0.794103 |0.791861|



## Author

| Birinder Singh | 
| ------------- | 
| [@Birinder1469](https://github.com/Birinder1469) | 