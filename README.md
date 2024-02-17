# Ex.No: 01 PLOT A TIME SERIES DATA
###  Date: 

# AIM:
To Develop a python program to Plot a time series data (Electric_Production).
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```py
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("Electric_Production.csv")
data["Date"]=pd.to_datetime(data["Date"])
plt.plot(data['Date'], data['Value'], label='Time Series Data')
plt.grid(True)
plt.title('Time Series Data Plot')
plt.xlabel('Date')
plt.ylabel('Value')
plt.legend()
plt.show()
```
# OUTPUT:
![alt text](image.png)]
# RESULT:
Thus we have created the python code for plotting the time series of given data.
