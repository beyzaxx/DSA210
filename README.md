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


## Statistical Test

- We used the Pearson correlation coefficient (r) to measure the strength and direction of the relationship.

- We also performed an Ordinary Least Squares (OLS) regression to check the results again.



## Results


The analysis focuses on the correlation between **Air Quality** and **Water Pollution** levels across different countries.

The following Python code was used to calculate the Pearson correlation coefficient:

```python
corr = df["AirQuality"].corr(df["WaterPollution"])
print(corr)
# Output: -0.454
```
Correlation coefficient: r = -0.454

p-value: < 0.05

Interpretation → There is a moderate negative link between air quality and water pollution:
as air quality gets better (higher score), water pollution usually goes down.


## Findings

Countries in Northern Europe, like Finland, Norway, and Sweden, have good air quality and low water pollution. In the Middle East and Caribbean, air quality is bad and water is more polluted, probably because of industries and oil-related activities. The negative link (-0.45) supports the idea that environmental quality in different areas is connected. These findings show that pollutants might come from the same sources and show the need for environmental policies that look at both air and water together.


## Limitations and Future Work

The data is from just one year (2021), so it doesn't show changes over time. Air and water quality measurements use different standards, which might cause differences in results. Correlation doesn't mean one thing causes the other — other factors like GDP, industry, and CO₂ emissions might give a better picture.


## Future directions

Add more detailed water quality data, like oxygen levels, chemical content, pH, and metals. Look at data over time, like from 2010 to 2025. Use machine learning models to predict pollution levels using region-specific information. Make a visual tool using Plotly or Dash to show the data clearly.


## Conclusion

The results show that the idea that air quality and water pollution are not connected is not true. Cleaner air is linked to cleaner water — showing how environmental systems are connected and why it's important to take a whole-system approach to pollution control.













