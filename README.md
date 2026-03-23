# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 02/02/2026
## Reg No: 212224240053

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt

df=pd.read_csv('/content/Tesla Dataset.csv')
df.shape

df1=df.head(100)
df1
```

<img width="743" height="510" alt="image" src="https://github.com/user-attachments/assets/93728eaf-d674-40df-843d-51196ac5d22d" />

```
df.info()
```

<img width="403" height="311" alt="image" src="https://github.com/user-attachments/assets/c1508b39-9ebd-4f6b-ad24-29a269562dde" />

```
df.describe()
```

<img width="808" height="358" alt="image" src="https://github.com/user-attachments/assets/a2dead90-9979-4815-9118-deee1aaaafc5" />

```
x=df1['Date']
y=df1['Open']

plt.figure(figsize=(10,6))
plt.bar(x,y)
plt.grid(True)
plt.title('Date vs Open')
plt.xlabel('Date')
plt.ylabel('Open')
plt.show()
```


# OUTPUT:

<img width="1065" height="680" alt="image" src="https://github.com/user-attachments/assets/febfab0b-3b72-4d03-ad0f-79b252945f56" />







# RESULT:
Thus we have created the python code for plotting the time series of given data.
