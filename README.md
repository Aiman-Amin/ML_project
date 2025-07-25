Real Estate: Data Integration, Cleaning API & Modeling Project
Project Objective
This project replicates a practical data science workflow by sourcing property data from two separate real estate APIs, followed by thorough cleaning, transformation, and integration of the datasets. The main aim is to develop an accurate predictive model for property pricing. A key part of the challenge involves deploying both the data preprocessing pipeline and the machine learning model as independent RESTful API endpoints. All components and code are documented and available within the associated GitHub repository.
APIs used for data collection
This project utilizes two distinct APIs to gather comprehensive property-related data:
•	ATTOM Property Data API
A commercial real estate API offering extensive property information. Data is retrieved via the official endpoint: API 1 Endpoint: https://www.attomdata.com/solutions/property-data-api/
•	Custom Simulated API (FastAPI)
A locally hosted API developed using FastAPI to emulate a secondary data source. It enriches the dataset with additional property attributes. Full implementation details can be found in the project repository.
These two sources ensure a diverse and realistic dataset for training and testing the predictive model.

Steps taken in data collection and cleaning
The data preparation phase involved gathering and refining property information from two sources:
•	Extracted property records in JSON format using the ATTOM Data API.
•	Combined both datasets into a single unified DataFrame for analysis.
•	Performed thorough data cleaning, which included:
o	Removing duplicate entries and records with missing values.
o	Standardizing and converting data types to ensure consistency.
o	Addressing missing fields and aligning schema across sources.
o	Eliminating irrelevant or redundant features that added no predictive value.
This process ensured a high-quality, structured dataset suitable for modeling.

Modeling approach and results
Three machine learning models were implemented and tested:
•	Decision Tree Regressor
•	Random Forest Regressor
•	XGBoost Regressor
Best Performing Model:
Random Forest Regressor delivered the most accurate results in terms of performance metrics (Performance metrics are documented in the provided code and analysis notebook).
