# Ex-08-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.

# CODE
```
#DEVELOPED BY : SWETHA P
#REGISTER NUMBER: 212222100053
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
tips_df=sns.load_dataset("tips")
tips_df
sns.barplot(data = tips_df,x = "total_bill",y = "day")
sns.relplot(data = tips_df,x = "total_bill", y="tip",hue = "smoker", style = "smoker")
sns.displot(data = tips_df,x = "total_bill", y="tip",hue = "smoker")
sns.barplot(data = tips_df,x = "total_bill", y="tip",hue = "smoker")
sns.kdeplot(data = tips_df, x ="total_bill", y = "tip", size ="size")
sns.relplot(data = tips_df, x ="total_bill", y = "tip", hue = "day", col = "time")
sns.relplot(data = tips_df, x = "total_bill",y = "tip", col="day",col_wrap=2)
sns.lineplot(x = "total_bill", y = "tip", data = tips_df, hue = "sex",
style = "sex",
markers = ["o","<"], legend = "auto")
```
# OUPUT
![Screenshot 2023-06-04 162234](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/a97123cf-9718-40e3-a41f-55ac43b00c9d)
![Screenshot 2023-06-04 162357](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/572061e3-50b4-4698-9f92-705fdb08ed25)
![Screenshot 2023-06-04 162420](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/de47fba0-a1c0-46ec-9263-d410cfdeb02f)
![Screenshot 2023-06-04 162443](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/d81388b7-2b6b-4b3c-8591-e58ee4a35669)
![Screenshot 2023-06-04 162502](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/8869bc41-063a-45b3-994d-75c36162da1b)
![Screenshot 2023-06-04 162638](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/ccaa7eaf-8a54-40a3-81e8-ffafe0500d37)
![Screenshot 2023-06-04 162704](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/de6908ae-4f6a-44d7-96ba-e207107b6b63)
![Screenshot 2023-06-04 162738](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/8b526873-4c78-4116-9e21-a2bca9237d61)
![Screenshot 2023-06-04 162756](https://github.com/swetha1510/Ex-08-Data-Visualization_1/assets/120623583/c49572f3-d1bc-4b9e-9a9a-47c903e46165)


# RESULT
Thus Data Visualization is performed on the given dataset and save the data to a file.


















