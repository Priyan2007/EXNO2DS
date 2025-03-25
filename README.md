![image](https://github.com/user-attachments/assets/d43090e4-661f-4424-a7c8-03138ef61866)# EXNO2DS
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
## Ctegorical data analysis
```
df.nunique()
```
![image](https://github.com/user-attachments/assets/8ad8dad4-d234-437d-a629-e4ea8045bc7c)
```
df["Survived"].value_counts()
```
![image](https://github.com/user-attachments/assets/0acab847-8d9e-4a90-a8af-bfd22194f5cb)
```
per=(df["Survived"].value_counts()/df.shape[0]*100).round(2)
per
```
![image](https://github.com/user-attachments/assets/ebfdb587-f0b4-46c8-83e6-6d2cef83057a)
```
sns.countplot(data=df,x="Survived")
```
![image](https://github.com/user-attachments/assets/27b9dea5-90b8-4962-b12e-e9183061f6a9)
```
df
```
![image](https://github.com/user-attachments/assets/0070c361-77d0-477b-8db6-e77ccf1996d9)
```
df.Pclass.unique()
```
![image](https://github.com/user-attachments/assets/dffe47c4-563e-43f4-838f-3cabc351ac3e)
```
df.rename(columns={'Sex':'Gender'},inplace=True)
df
```
![image](https://github.com/user-attachments/assets/5152d58d-495d-4e9a-acb7-5b58fab2c2e2)
## Bivariate Analysis










# RESULT
        <<INCLUDE YOUR RESULT HERE>>
