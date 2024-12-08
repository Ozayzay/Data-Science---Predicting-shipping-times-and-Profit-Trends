# Sales Record Analysis and Machine Learning
This project processes and analyzes sales data to generate insights and apply machine learning models to predict shipping times. The project involves cleaning data, exploratory data analysis, statistical testing, and machine learning model training.



# Table of Contents
- [Setup]
- [Structure]
- [Files Produced]
- [Running the Code]
- [Questions answered]


# Setup
# Required Libraries
Make sure you have Python installed along with the following libraries:
- `matplotlib`
- `pandas`
- `numpy`
- `scipy`
- `scikit-learn`


# Structure 
- All of the functions are being run in main.py while their implementations are in clean_data.py and generate_plots.py 


# Files Produced 
- At the begining of main.py we are running function cleanAndSortData(dataFrame_raw, output_file_name) that creates SalesRecordClean.csv
which is a clean dataframe that is used for the data analysis, to learn about cleanAndSortData() look at [ETL / Step 2]


# Running the Code
Run The code using following command:
    - python3 main.py [INPUT_PATH]

Which in our case looked like:
    - python3 main.py SalesRecords/SalesRecords_5m.csv

Download Dataset - 
https://excelbianalytics.com/wp/downloads-18-sample-csv-files-data-sets-for-testing-sales/



# Questions Answered 
- Q1: Can we Predict how many days it will take to ship items based on features such as order priority, product type and region.

- Q2: Does unit price have an impact on Profit?




