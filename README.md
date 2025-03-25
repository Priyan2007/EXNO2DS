# EXNO2DS
# AIM:
      To perform Exploratory Data Analysis on the given data set.
      
# EXPLANATION:
  The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.
  
# ALGORITHM:
STEP 1: Import the required packages to perform Data Cleansing,Removing Outliers and Exploratory Data Analysis.

STEP 2: Replace the null value using any one of the method from mode,median and mean based on the dataset available.

STEP 3: Use boxplot method to analyze the outliers of the given dataset.

STEP 4: Remove the outliers using Inter Quantile Range method.

STEP 5: Use Countplot method to analyze in a graphical method for categorical data.

STEP 6: Use displot method to represent the univariate distribution of data.

STEP 7: Use cross tabulation method to quantitatively analyze the relationship between multiple variables.

STEP 8: Use heatmap method of representation to show relationships between two variables, one plotted on each axis.

## CODING AND OUTPUT
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("/content/titanic_dataset.csv")
df
```
![image](https://github.com/user-attachments/assets/e2d2d875-46d9-42e9-93ad-fe067e648502)
```
df.info()
```
![image](https://github.com/user-attachments/assets/e99e26de-9426-4b2f-85a3-d90b8ffce2c0)
```
df.shape
```
![image](https://github.com/user-attachments/assets/e55c4a25-4f3c-458f-a374-98bd1b4224a4)
```
df.set_index("PassengerId",inplace=True)
df.describe()
```
![image](https://github.com/user-attachments/assets/6b250da6-81b4-4ec7-a9b2-7c6bc5930af7)
```
df.shape
```
![image](https://github.com/user-attachments/assets/2c961098-5e20-412d-a2c6-db2e55f7f2f8)




# RESULT
        <<INCLUDE YOUR RESULT HERE>>
