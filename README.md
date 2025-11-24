# DSA210

## Project Overview

I am a student at Sabancı University, Beyza Iğdır (22578), and this is my DSA210 term project.
In this project, I want to find out if there is a strong connection between air quality and water pollution levels in different countries around the world.
I will use the dataset called “World’s Air Quality and Water Pollution” from Kaggle to see if cleaner air is linked to cleaner water, and whether improving the environment in one area might also help improve it in another.
The project will involve cleaning the data, doing some initial analysis to understand the data better, checking for correlations, and creating visualizations using Python.

## Motivation

Environmental pollution is one of the biggest dangers to human health and the balance of nature.
Out of all the types of pollution, air and water pollution are especially serious because they come from the same sources — like using fossil fuels, making manufacturing waste, and not having good environmental rules.
This project looks at whether air quality and water pollution are connected in different countries.
If places with cleaner air also have cleaner water, it would show that improving one part of the environment might help the other as well. This idea is important for making the world more sustainable and for creating better environmental policies.

## Data Source

The data used in this project is called “World’s Air Quality and Water Pollution,” which is available on Kaggle. It has 3963 rows and 5 columns, showing environmental data from cities all around the world collected in 2021.

### **Dataset Overview**

This dataset contains global environmental indicators for 3963 cities with the following features:

| Feature | Description | Example |
|----------|-------------|----------|
| City | Name of the city | New York City |
| Region | Province or state | New York |
| Country | Country name | United States of America |
| AirQuality | Air quality index (0 = poor, 100 = excellent) | 46.81 |
| WaterPollution | Water pollution index (0 = clean, 100 = extreme pollution) | 49.50 |

Source: [Kaggle – World’s Air Quality and Water Pollution Dataset](https://www.kaggle.com/datasets/ryotapy/worlds-air-quality-and-water-pollution-dataset)


## Data Analysis


### Objective

We want to check if there is a statistically significant connection between air quality and water pollution in different parts of the world.

### Hypotheses

Null Hypothesis (H₀): There is no meaningful link between air quality and water pollution (ρ = 0).
Alternative Hypothesis (H₁): There is a meaningful link between air quality and water pollution (ρ ≠ 0).


## Methods


Data Cleaning: We took out quotation marks from the Region and Country columns, and made sure there were no missing values.
Aggregation: We found the median values for AirQuality and WaterPollution at the country level.

## Visualization:

- Bar charts showing the top and bottom 50 countries in terms of air and water quality.

- A scatter plot to show how air quality relates to water pollution overall.


## Statistical Analysis

Pearson correlation coefficient

Ordinary Least Squares (OLS) regression for additional validation

All steps will be conducted using Python libraries such as pandas, seaborn, matplotlib, and statsmodels.

 ## Expected Outcomes

The project is expected to:

Reveal the strength and direction of the relationship between air and water pollution

Provide descriptive comparisons across countries

Highlight potential patterns in environmental performance

Offer insights that may encourage integrated environmental policy approaches













