# Exercise 5: Data analysis with pandas (10 points)

In this exercise, we will be doing data analysis using [pandas - the Python Data Analysis Library](http://pandas.pydata.org/). So far, we have only used example data stored in list variables, and this week we will be loading data files and interacting with actual data sets. 

In this exercise you are asked to analyze air temperature data from Kumpula, Helsinki (in Southern Finland) and Rovaniemi (a city in northern Finland) and to explore how their summer temperatures differed in 2017.

## Completing the exercise

- **Remember to save and commit your changes locally, and push your changes to GitHub after each major change**!
- **We are [working in pairs](https://geo-python-upd.readthedocs.io/en/latest/lessons/L2/why-pairs.html) on this exercise**, and we will only grade the repository of the member of your pair that is responsible for this week's exercise.

## Where to find help

- Review the [materials for Lesson 5](https://geo-python-upd.readthedocs.io/en/latest/lessons/L5/overview.html)
- Check out the [hints for this week's exercise](https://geo-python-upd.readthedocs.io/en/latest/lessons/L5/exercise-5.html#exercise-5-hints) if you're having trouble.

## Before you start

### Clone the Exercise 5 repository

Before starting to work with the problems for this week, you should start a new JupyterLab instance and dowsnload your own Exercise 5 repository (e.g., `exercise-5-jdaled`) from the Github Classroom link, and upload the notebooks and data to the Binder instance.

### Input data

We will use NOAA weather data obtained from [here](https://www.ncdc.noaa.gov/cdo-web/datatools/records). The data has been stored in a CSV file (comma delimited text file) which is stored in this repository: [data/ph_temp_data.csv](data/ph_temp_data.csv).

You can read the full description of the data and all the attributes [here](https://www.ncdc.noaa.gov/cdo-web/datasets#GHCND). 

The first five rows of the data look like following:

```
STATION,NAME,LATITUDE,LONGITUDE,ELEVATION,DATE,TEMP,MAX,MIN
RPM00098646,"MACTAN CEBU INTERNATIONAL, RP",10.308,123.979,9.400,2017-01-01,79.700,86.000,***
RPM00098646,"MACTAN CEBU INTERNATIONAL, RP",10.308,123.979,9.400,2017-01-02,79.880,85.640,***
RPM00098646,"MACTAN CEBU INTERNATIONAL, RP",10.308,123.979,9.400,2017-01-03,82.400,88.520,76.640
RPM00098646,"MACTAN CEBU INTERNATIONAL, RP",10.308,123.979,9.400,2017-01-04,82.040,89.240,***
```

**NOTICE**: the data includes \* that represent NoData values.

The most important attributes for this exercise are:

 - **STATION** = the station ID number
   - RPM00098646 : Cebu
   - RP000098755 : Hinatuan
 - **Date** = Year-MM-DD
 - **TEMP** = Temperature in Fahrenheit
 - **MAX** = Maximum temperature in Fahrenheit
 - **MIN** = Minimum temperature in Fahrenheit
 
## Start working

There are three graded problems in this week's exercise and one optional problem.

1. [Problem 1: Basic statistics (2 points)](Exercise-5-problem-1.ipynb)
2. [Problem 2: Data manipulation and subsetting (4 points)](Exercise-5-problem-2.ipynb)
3. [Problem 3: Data analysis (4 points)](Exercise-5-problem-3.ipynb)
4. [Problem 4: Data aggregation (*optional*, 0 points)](Exercise-5-problem-4.ipynb)