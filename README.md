## Developed by:SABARI S
## Register No:212222240085
## Date:
# Ex.No: 01A PLOT A TIME SERIES DATA
 

# AIM:
To Develop a python program to Plot a time series data of Air Quality in Top Cities
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

data = pd.read_csv("/content/data_date.csv")

data['Date'] = pd.to_datetime(data['Date'])

plt.figure(figsize=(10,6))
plt.plot(data['Date'], data['AQI Value'], label='AQI Value', color='black')


plt.title('AIR QUALITY')
plt.xlabel('Date')
plt.ylabel('AQI Value')
plt.legend()
plt.show()
```




# OUTPUT:

![Screenshot 2024-09-18 183204](https://github.com/user-attachments/assets/69985c72-dfc6-413a-921c-ec4787985f12)




# RESULT:
Thus,the python code for plotting the time series of given data.
