# Chicago E-Scooter distribution optimization

This project focuses on analyzing the E-Scooter Trips dataset provided by the City of Chicago. 
The dataset contains information about e-scooter trips that took place in 2020. 
The dataset can be accessed at [E-Scooter Trips 2020](https://data.cityofchicago.org/Transportation/E-Scooter-Trips-2020/3rse-fbp6).

## Project Overview

The main objectives of this project are:

1. Optimize the E-Scooter ditribution across the city
2. Optimize the distribution across the day, in consideration of rush hours 

## Experiments

The following steps were conducted on the dataset:

1. **Data Cleaning:** In this phase, we performed various cleaning operations to ensure the data is consistent and ready for analysis. This involved handling missing values, removing duplicates, and correcting any inconsistencies or errors in the data.

2. **Data Transformation:** To make the data more suitable for analysis, we transformed it into a structured format. This included converting data types, encoding categorical variables, and creating new features as required.

3. **Vendor Prediction:** Using machine learning techniques, we built a model to predict the vendor based on the start community area. This task aimed to identify patterns and factors that contribute to vendor selection in different community areas.
The models we used are Random Forest and Descision trees.

4. **End Area Prediction:** Another prediction task involved predicting the end community area using the start community area and start day. This analysis aimed to understand the relationship between the start community area, start day, and the final destination of the e-scooter trips.
The models we used are Random Forest and Descision trees.

5. **End community area prediction:** Another prediction involved predicting the end community area using the start community area and start hour.
The models we used are XGBoost and KNN

**Purpose:** The purpose of all those experiments is to optimize the distribution
Vendor - to find in which area the scooters of each vendor are most used
Start community and end community: To decide where to distribute the scooters in the most efficient way


## Dependencies

The project relies on the following libraries and packages:

- Python 3.7 or above
- pandas
- numpy
- matplotlib
- xgboost
- scikit-learn

Please refer to the `requirements.txt` file for specific versions of the packages used in this project.

## Usage

To run the project, follow these steps:

1. Clone or download the repository.
2. Install the required dependencies by running `pip install -r requirements.txt`.
3. Download the E-Scooter Trips 2020 dataset from the [City of Chicago Data Portal](https://data.cityofchicago.org/Transportation/E-Scooter-Trips-2020/3rse-fbp6) and place it in the `data` directory.
4. Open the Jupyter Notebook provided and execute the code.



