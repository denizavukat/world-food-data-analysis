
# World Food-Feed Production Analysis

## Overview
This project explores global food and feed production with an emphasis on analyzing environmental impacts, production trends, and predicting emissions using machine learning models. Our aim is to understand global food production patterns, categorize countries based on production capabilities, and predict emissions associated with food production.

## Authors
- Sena Deniz Avukat
- Yuqian Gao
- Krisztina Rostás
- Tapio Uzal

## Project Objectives
1. **Clustering Countries Based on Food Production and Geographical Location**: Identify similarities between countries regarding their production capabilities and geographical locations.
2. **Analyzing Emissions from Food Production**: Analyze the environmental impact of each food category and build a prediction model for total emissions.

## Research Questions
- How can we cluster countries based on food production volumes in different categories?
- How does food and feed production compare to each other?
- Which food categories generate the highest emissions?
- How has food production in countries evolved over the years?
- Can we predict total emissions based on current data?

## Methodology
1. **Exploratory Data Analysis (EDA)**: Analyzed two datasets sourced from Kaggle:
   - *Who Eats the Food We Grow?* - Provides insight into global food production between 1961-2013.
   - *Environmental Impact of Food Production* - Contains environmental data for 43 common foods.
2. **Data Cleaning**: Performed standardization of country names, handled missing values, and reshaped the data for analysis.
3. **Prediction Using Regression Models**: Used four regression models (`RandomForestRegressor`, `DecisionTreeRegressor`, `AdaBoostRegressor`, and `LinearRegression`) to predict total emissions.
4. **Country Clustering**: Clustered countries using K-means based on total and average production, latitude, and longitude to determine production and geographical similarities.

## Results and Discussion
- **Country Clustering**: Countries were clustered into four groups based on production and geographical features, which revealed insights into different production capacities globally.
- **Emission Analysis**: The highest emissions were attributed to animal products, with bovine meat being the largest emitter. Emission data was visualized to highlight differences between categories.
- **Regression Models**: Linear and decision tree regressors performed well in predicting emissions, as shown by low RMSE values.

## Technologies Used
- **Python Libraries**: Pandas, Scikit-learn, Pycountry, Matplotlib
- **Clustering Algorithms**: K-means
- **Regression Models**: RandomForest, DecisionTree, AdaBoost, Linear Regression



## Installation
1. Clone the repository:

   ```bash
   git clone https://github.com/denizavukat/World-Food-Feed-Production.git





2. Create a virtual environment and activate it:

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`



3. Install the required packages:

    ```bash
    pip install -r requirements.txtResults



## Results

* Detailed results, visualizations, and discussions are available in the results/ directory.

* Clustering results are visualized as maps to illustrate production similarities across countries.

License

This project is licensed under the MIT License.

Acknowledgements

Data sourced from Kaggle: Who Eats the Food We Grow? and Environmental Impact of Food Production.


