## Developed by:AJAY ASWIN M
## Register No:212222240005
## Date:
# Ex.No: 01A PLOT A TIME SERIES DATA
 

# AIM:
To Develop a python program to Plot a time series data of Petrol Price in Top Cities
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the Petrol Price dataset using the pandas
3. Plot the data according to need and can be altered monthly, or yearly.
4. Display the graph.
5. End of the Program.
# PROGRAM:
```py
import pandas as pd
import matplotlib.pyplot as plt

data = pd.read_csv("/content/petrol.csv")

data['Date'] = pd.to_datetime(data['Date'])

plt.figure(figsize=(10,6))
plt.plot(data['Date'], data['Chennai'], label='Chennai', color='black')
plt.plot(data['Date'], data['Mumbai'], label='Mumbai', color='blue')
plt.plot(data['Date'], data['Delhi'], label='Delhi', color='Red')

plt.title('Petrol Price in Top Cities')
plt.xlabel('Date')
plt.ylabel('Petrol Price')
plt.legend()
plt.show()
```




# OUTPUT:


![petrol](https://github.com/user-attachments/assets/30019de2-b4b0-4f70-ab98-377d6d15bf5a)




# RESULT:
Thus,the python code for plotting the time series of given data.
