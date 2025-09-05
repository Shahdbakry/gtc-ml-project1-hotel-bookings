# Hotel Booking Data Cleaning & Preprocessing

# Project Overview

This project is part of the GTC Machine Learning Track – Project 1.
The main goal is to clean and preprocess raw hotel booking data (hotel_bookings.csv) so it is ready for building a machine learning model that can predict booking cancellations.

We are not training the final model here — the focus is on data quality and preprocessing, since clean data directly impacts the success of predictive models.

# Objectives

1- Exploratory Data Analysis (EDA)

- Summarize data with .info() and .describe()

- Identify missing values and visualize them with heatmaps

- Detect outliers in key columns like adr and lead_time

2- Data Cleaning

- Handle missing values (company, agent, country, children)

- Remove duplicate rows

- Cap extreme outliers (adr > 1000)

- Fix incorrect datatypes (e.g., date columns)

3- Feature Engineering

- Create new features:

- total_guests = adults + children + babies

- total_nights = stays_in_weekend_nights + stays_in_week_nights

- is_family (binary flag)

4- Preprocessing

- Encode categorical variables:

- One-Hot Encoding (for low-cardinality columns like meal)

- Frequency Encoding (for high-cardinality column country)

- Drop leakage columns (reservation_status, reservation_status_date)

- Split data into training and test sets (80/20)

# Results

- Dataset cleaned and missing values handled

- Outliers capped (e.g., ADR > 1000)

- New features engineered (total_guests, total_nights, is_family)

- Categorical variables encoded properly

- Train-test split ready for modeling
