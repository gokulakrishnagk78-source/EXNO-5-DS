# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
 import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

sns.set(style='whitegrid')
plt.rcParams['figure.figsize'] = (10, 6)

data = pd.read_csv("C:\\Users\\krishna\\Downloads\\bank_marketing (1).csv")

plt.hist(data['age'], bins=20, color='skyblue', edgecolor='black')
plt.title('Age Distribution')
plt.xlabel('Age')
plt.ylabel('Frequency')
plt.grid(axis='y', linestyle='--', alpha=0.7)
plt.show()

sns.countplot(x='job', data=data, palette='Set2')
plt.title('Job Distribution')
plt.xticks(rotation=45)
plt.grid(axis='y', linestyle='--', alpha=0.7)
plt.show()

sns.boxplot(x='marital', y='balance', data=data, palette='Set3')
plt.title('Balance by Marital Status')
plt.show()

sns.violinplot(x='education', y='age', data=data, palette='Pastel1')
plt.title('Age Distribution by Education')
plt.xticks(rotation=45)
plt.show()

sns.heatmap(data[['age', 'balance', 'duration', 'campaign', 'pdays', 'previous']].corr(), annot=True, cmap='coolwarm', linewidths=0.5)
plt.title('Correlation Matrix')
plt.show()
```
#OUTPUT:
![Screenshot_17-10-2025_114356_localhost](https://github.com/user-attachments/assets/7151753e-fb26-4f5d-a2bb-bd6bbc078d95)
![Screenshot_17-10-2025_114415_localhost](https://github.com/user-attachments/assets/21caf862-cf47-4a60-a2e4-429616368d6e)
![Screenshot_17-10-2025_114519_localhost](https://github.com/user-attachments/assets/910732f7-6fbc-4dd6-9d2d-584c87a5b628)
![Screenshot_17-10-2025_114533_localhost](https://github.com/user-attachments/assets/22d6e2bb-c135-4154-bd01-1c73fd069da9)
![Screenshot_17-10-2025_114415_localhost](https://github.com/user-attachments/assets/4de8111f-1904-4944-a61d-d8b361816640)





# Result:
 data visualization process for the sample dataset is performed successfully
