# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("Loan_data.csv")
df.head(5)

df.describe()

df.info()

df.tail()

df.shape
df.columns

# To check Null values
df.isnull().sum()

# To check duplication
~df.duplicated()

# Outlier detection
sns.boxplot(x="LoanAmount", data=df)

# Handling Missing Values
df['LoanAmount']

# OUPUT
![Screenshot 2023-03-19 012731](https://user-images.githubusercontent.com/121115650/226135301-37b45568-4c96-46b0-930f-8b4cc9a06314.png)
![Screenshot 2023-03-19 012753](https://user-images.githubusercontent.com/121115650/226135360-b145f6fd-78cb-4a69-99dc-7bfc3085f3d9.png)
![Screenshot 2023-03-19 012807](https://user-images.githubusercontent.com/121115650/226135376-c48549f5-3920-4f49-a35b-fd42938bc00f.png)
![Screenshot 2023-03-19 012855](https://user-images.githubusercontent.com/121115650/226135416-d15f03df-4341-43cb-bb03-e16388369cde.png)
![Screenshot 2023-03-19 012948](https://user-images.githubusercontent.com/121115650/226135452-64427bf4-e556-4c71-b61d-9961e93f9c10.png)
![Screenshot 2023-03-19 013000](https://user-images.githubusercontent.com/121115650/226135589-ae477eab-bd38-42dc-b993-f3d3083e497a.png)
![Screenshot 2023-03-19 013011](https://user-images.githubusercontent.com/121115650/226135777-21b0db07-34f5-4ffe-affb-763a42bafc66.png)
![Screenshot 2023-03-19 013023](https://user-images.githubusercontent.com/121115650/226135794-475a24db-4674-461d-9979-63d65aede8a0.png)
![Screenshot 2023-03-19 013033](https://user-images.githubusercontent.com/121115650/226135811-fa9b5666-1beb-4143-8818-30b4daa117a8.png)

# Result
Thus the given data is read,cleansed and cleaned data is saved into the file.







