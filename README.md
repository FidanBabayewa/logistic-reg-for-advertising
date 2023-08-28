# Logistic Regression Project

This project involves working with a synthetic advertising dataset to build a predictive model. The goal is to determine whether an internet user will click on an advertisement based on various user features. The dataset contains information such as daily time spent on the site, age, area income, daily internet usage, and more.

## Dataset Features

The dataset includes the following features:

- **Daily Time Spent on Site:** Amount of time a consumer spends on the site in minutes.
- **Age:** Age of the customer in years.
- **Area Income:** Average income of the geographical area of the consumer.
- **Daily Internet Usage:** Average minutes per day that the consumer spends on the internet.
- **Ad Topic Line:** Headline of the advertisement.
- **City:** City of the consumer.
- **Male:** Indicates whether the consumer is male (1) or not (0).
- **Country:** Country of the consumer.
- **Timestamp:** Time at which the consumer clicked on the ad or closed the window.
- **Clicked on Ad:** Binary value (0 or 1) indicating whether the consumer clicked on the ad.

## Project Steps

### Import Libraries
The project begins by importing necessary Python libraries for data analysis and visualization, including numpy, pandas, matplotlib, and seaborn.

### Loading Data
The `advertising.csv` file is read into a pandas DataFrame named `ad_data`.

### Exploratory Data Analysis
Exploratory data analysis (EDA) is performed using seaborn to create several visualizations:
- Histogram of the age distribution.
- Jointplot displaying the relationship between Area Income and Age.
- Jointplot with kernel density estimate (KDE) distributions of Daily Time spent on site vs. Age.
- Jointplot of 'Daily Time Spent on Site' vs. 'Daily Internet Usage'.
- Pairplot to visualize relationships among various features, with the hue defined by the 'Clicked on Ad' column.

### Logistic Regression
The project proceeds to train a logistic regression model. Steps include:
- Splitting the data into a training set and a testing set using the `train_test_split` function.
- Training and fitting a logistic regression model using the training set.

### Predictions and Evaluation
The trained model is then used to make predictions on the testing data. A classification report is generated to evaluate the performance of the model in predicting whether a user will click on an ad.

## Conclusion
This project demonstrates the process of working with a synthetic advertising dataset, performing exploratory data analysis, training a logistic regression model, and evaluating its performance. By following the provided steps, you can gain insights into user behavior and create a predictive model for click-through rates on advertisements.

Feel free to explore and modify the project as needed to further enhance your understanding of logistic regression and data analysis.
