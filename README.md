# Module_14_Challenge

---

## Establish baseline performance and tune trading algorithm

---

## Analysis

As a financial advisor at one of the top five financial advisory firms in the world, this analysis focuses on keeping the firm in a competetive stance by improving the existing algorithmic trading systems.  This will be accomplished by utilizing machine learning algorithms with consideration of additional data.

---

## Analytical Results

Baseline Model:

Utilizing the emerging market information from the csv file, use the following parameters:
    * short window = 4
    * long window = 100
    * SVC classifier model
    * focus on Predicted values, Actual Returns, and Strategy Returns

The baseline model's accuracy was 55%, with the precision landing at 43% and 56% for (-1) and (1), repectively.  The recall scores landed at 4% and 96% for (-1) and (1), repectively. 

![classification_report](/Images/Classification_report_svm)

![plot_baseline](/Images/Act_vs_Strat_Baseline)

Alternative Model:
    * short window = 4
    * long window = 100
    * LR classifier model
    * focus on Predicted values, Actual Returns, and Strategy Returns

The alternative model's accuracy was 52%, with the precision landing at 44% and 56% for (-1) and (1), repectively.  The recall scores landed at 33% and 66% for (-1) and (1), repectively. 

![classification_report](/Images/Classification_report_LR)

![plot_baseline](/Images/Act_vs_Strat_lr)

---

## Technologies

This model was written using Python 3.7 with the following imports:

'''
    * import pandas as pd
    * import numpy as np
    * from pathlib import Path
    * import hvplot.pandas
    * import matplotlib.pyplot as plt
    * from sklearn import svm
    * from sklearn.preprocessing import StandardScaler
    * from pandas.tseries.offsets import DateOffset
    * from sklearn.metrics import classification_report
'''

## Usage

To view this model, clone the repository and run the .upynb file.

---

## Contributors

Brought to you by ABolla, FA

---

##  License

MIT




