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

# NON NULL AFTER
![S11](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/a4b05849-3e9c-49cd-a464-4e1f4677b3b6)

![S12](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/457e0703-0bfa-45d2-9b45-91607fedfabe)

# OUTPUT:
# For loan_data:
# DATA
![S1](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/dace3774-945a-406c-9a80-57f5fd52a12e)



![S2](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/a70c293d-0e95-4b3e-a53d-d0b7dd6f0841)


![S3](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/56283896-becf-4f5d-a581-58c85f211ac7)


# NON NULL BEFORE

![S4](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/5e01431a-43c8-4d8f-b3f2-ac25218ef988)


![S5](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/d9662985-7953-4b92-a039-0617371eca3b)
# MODE

![S6](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/969248ef-262d-4bf8-8c82-8ff271affbcb)
# MEAN

![S7](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/1cef2831-35a8-4704-ae6d-e27f8c3d12d5)

# MEDIAN
![S9](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/9b846d73-7a57-49ce-8a30-fecfd34106d1)

# NON NULL AFTER

![S10](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/e2c0b60f-4a70-4c5e-8440-6e5bfbb2f0e6)




![S11](https://github.com/Pavithraramasaamy/ODD2023-Datascience-Ex01/assets/118596964/e5cb44d6-2f79-4fb7-8f0d-d9357394ab03)


