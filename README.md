# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 
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

df=pd.read_csv('/content/price_of_healthy_diet_clean.csv')
df.shape

df1=df.head(100)
df1
```

<img width="1305" height="327" alt="image" src="https://github.com/user-attachments/assets/3f6c3227-b925-4b70-8f7f-9a9e18cac44f" />

```
df.info()
```

<img width="699" height="400" alt="image" src="https://github.com/user-attachments/assets/a351c1cb-9f6c-408e-94db-5698df835124" />

```
df.describe()
```

<img width="1272" height="293" alt="image" src="https://github.com/user-attachments/assets/685b5a15-590e-486b-9701-ceee6507768a" />

```
x=df1['year']
y=df1['cost_healthy_diet_ppp_usd']

plt.figure(figsize=(10,6))
plt.bar(x,y)
plt.grid(True)
plt.title('year vs cost_healthy_diet_ppp_usd')
plt.xlabel('year')
plt.ylabel('cost_healthy_diet_ppp_usd')
plt.show()
```

# OUTPUT:

<img width="1027" height="673" alt="image" src="https://github.com/user-attachments/assets/208ad915-c982-45a3-9198-18339eb6e05b" />







# RESULT:
Thus we have created the python code for plotting the time series of given data.
