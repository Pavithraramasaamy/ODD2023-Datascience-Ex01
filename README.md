# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE
#For Data_set
```python
import pandas as pd
df=pd.read_csv("/content/Data_set(1).csv")
print(df)

df.head(5)

df.info()

df.isnull()

df.isnull().sum()

df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
df.head()

df['rating']=df['rating'].fillna(df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()

df.head()

df['watchers']=df['watchers'].fillna(df['watchers'].median())
df.head()

df.info()

df.isnull().sum()

#For loan_data:
import pandas as pd
df=pd.read_csv("/content/Loan_Data.csv")
print(df)

df.head(5)

df.info()

df.isnull()

df.isnull().sum()

df['Loan_ID']=df['Loan_ID'].fillna(df['Education'].mode()[0])
df['Education']=df['Education'].fillna(df['Education'].mode()[0])
df['Married']=df['Married'].fillna(df['Education'].mode()[0])
df.head()

df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean())
df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())
df.head()

df.head()

df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].median())
df.head()

df.info()

df.isnull().sum()
```
# OUTPUT:
# For data_set:
# DATA
![S1](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/6620bc88-16bf-49cc-b55f-0666f0a42420)

![S2](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/cfa63996-7964-4c7e-b074-b40d56339919)

# NON NULL BEFORE

![S4](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/21d010fc-0438-4f6d-b900-52695e73e2d1)


![S5](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/97d1a886-559a-426b-8aa2-28610bee288e)

![S6](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/b00773a8-554e-41c1-a72b-17b70177c931)
# MODE

![S7](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/e904bac7-1680-45d2-9a77-b60a8d04e5c5)
# MEAN

![S8](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/2baff34b-a585-4679-9db5-26220c99471b)

# MEDIAN

![S10](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/c69839cb-6f56-47f0-a0e2-02af920eb9ef)

#NON NULL AFTER
![S11](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/a4b05849-3e9c-49cd-a464-4e1f4677b3b6)

![S12](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/457e0703-0bfa-45d2-9b45-91607fedfabe)



