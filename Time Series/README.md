# Forecasting PM2.5 Value

PM2.5 is an air pollutant that is a concern for people's health when levels in air are high. PM2.5 are tiny particles in the air that reduce visibility and cause the air to appear hazy when levels are elevated. Outdoor PM2.5 levels are most likely to be elevated on days with little or no wind or air mixing. The New York State Departments of Health (DOH) and Environmental Conservation (DEC) alert the public by issuing a PM2.5 Health Advisory when PM2.5 concentrations in outdoor air are expected to be unhealthy for sensitive groups.

## Data

**Data Source** = https://archive.ics.uci.edu/ml/datasets/Beijing+PM2.5+Data

The dataset time period is between Jan 1st, 2010 to Dec 31st, 2014.

Attribute Information:

1. No: row number
2. year: year of data in this row
3. month: month of data in this row
4. day: day of data in this row
5. hour: hour of data in this row
6. pm2.5: PM2.5 concentration (ug/m^3)
7. DEWP: Dew Point
8. TEMP: Temperature
9. PRES: Pressure (hPa)
10. cbwd: Combined wind direction
11. Iws: Cumulated wind speed (m/s)
12. Is: Cumulated hours of snow
13. Ir: Cumulated hours of rain

## Data Preprocessing

I dropped data without PM2.5 values (missing values). Since the data was sorted by time, i dropped No, year, month, day, and hour attributes. I also dropped cbwd to simplify data preprocessing since it is a categorical attribute so this project didn't do one hot encoding to handle categorical attributes.

Then, I transformed data into time series data. In this project i use 10 consecutive data before the target values. You can see the illustration below:

![alt text](https://github.com/adrinta/dicoding-machine-learning-developer/blob/main/Time%20Series/Assets/Data%20Transformation.png?raw=True)


## Model Architecture

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Time%20Series/Assets/Model%20Architecture.png)


## Results

**Training Graph**

![alt text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Time%20Series/Assets/training%20graph.png)

**Actual VS Prediction**

![alt_text](https://raw.githubusercontent.com/adrinta/dicoding-machine-learning-developer/main/Time%20Series/Assets/actual%20and%20prediction.png)

**Mean Absolute Error**

|Data|MAE|
|---|---|
|Train|12.599|
|Test|11.185|


