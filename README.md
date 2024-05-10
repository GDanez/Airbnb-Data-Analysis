# Project Title: Text and Predictive Analysis of Airbnb US Listings Using PySpark

## Description
Advanced Text and Predictive Analysis of US Listings Using PySpark is a data analytics project focused on analyzing listing data across the United States. This project leverages the power of Apache Spark, utilizing its PySpark module, to handle large datasets with complex variations and perform extensive data preprocessing, exploratory analysis, and advanced text processing for sentiment analysis and topic detection.

## Objective
Our primary goal is to develop predictive models capable of estimating listing prices based on key characteristics, thereby providing insights into factors that influence pricing dynamics in the U.S. while also performing sentiment analysis on key features that could influence pricing.

## Key Features and Workflow:  
**Data Preprocessing and Cleaning**: Initial data cleaning to handle missing values including NaN and Null values. Imputed values using median, mean and replacing null with 0 for numerical variables depending on the situation. Replaced missing values of text columns as empty strings, while on categorical variables a new category named "Unknown" was created. Zip code is filled with the most frequent occuring zipcode of the specific city and information from another dataset was used to validate the city names in the dataset and to correctly identify the states of each city.  
**Exploratory Data Analysis (EDA)**: Detailed exploration of the dataset to uncover patterns, trends, and correlations between different variables.  
**Sentiment Analysis**: Utilizing text columns to perform sentiment analysis, helping to understand the emotions and sentiments expressed in listing descriptions, house rules, interaction, transit, etc.  
**Transit-based Listing Recomendation System**: In order to enhance user experience and facilitate easier access to desired listings, we implemented a transit-based listing recommendation system. This system allows users to specify their transit preferences, and based on their input, the system recommends the top 10 listings that best match their criteria.  
**Feature Importance and Selection**: Evaluating the importance of various features in the dataset, followed by selecting the most impactful features to improve model performance.  
**Predictive Modeling with Decision Trees**: Developing a regression model using decision trees to predict listing prices based on the selected features.  
**Recomendation System**: After selecting the best features for our recommendation system, we are implementing an advanced algorithm using the MinHashLSH model to recommend the top 3 listings that closely match the input listing provided by the user.  
**Technologies Used**:  
Apache Spark / PySpark: For distributed data processing.  
Python on google colab: For code and additional data manipulation.  

**Purpose**: This project is designed as a practical application of big data tools providing real estate analytics, suitable for academic purposes, real estate market analysis, and data science training.  
  
**The csv files that were used for this project were retrieved from here**:  
The Airbnb listing which is the main file that was used for this analysis is available in this link: https://public.opendatasoft.com/explore/dataset/airbnb-listings/table/?disjunctive.host_verifications&disjunctive.amenities&disjunctive.features  
Us cities is the second csv file that we used to fill in missing values while we also obtained extra information and performed extra analysis:  https://simplemaps.com/data/us-cities  
