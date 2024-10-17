World Food-Feed Production Analysis

Overview

This project explores global food and feed production with an emphasis on analyzing environmental impacts, production trends, and predicting emissions using machine learning models. Our aim is to understand global food production patterns, categorize countries based on production capabilities, and predict emissions associated with food production.

Authors

Sena Deniz Avukat

Yuqian Gao

Krisztina Rostás

Tapio Uzal

Project Objectives

Clustering Countries Based on Food Production and Geographical Location: Identify similarities between countries regarding their production capabilities and geographical locations.

Analyzing Emissions from Food Production: Analyze the environmental impact of each food category and build a prediction model for total emissions.

Research Questions

How can we cluster countries based on food production volumes in different categories?

How does food and feed production compare to each other?

Which food categories generate the highest emissions?

How has food production in countries evolved over the years?

Can we predict total emissions based on current data?

Methodology

Exploratory Data Analysis (EDA): Analyzed two datasets sourced from Kaggle:

Who Eats the Food We Grow? - Provides insight into global food production between 1961-2013.

Environmental Impact of Food Production - Contains environmental data for 43 common foods.

Data Cleaning: Performed standardization of country names, handled missing values, and reshaped the data for analysis.

Prediction Using Regression Models: Used four regression models (“RandomForestRegressor”, “DecisionTreeRegressor”, “AdaBoostRegressor”, and “LinearRegression”) to predict total emissions.

Country Clustering: Clustered countries using K-means based on total and average production, latitude, and longitude to determine production and geographical similarities.

Results and Discussion

Country Clustering: Countries were clustered into four groups based on production and geographical features, which revealed insights into different production capacities globally.

Emission Analysis: The highest emissions were attributed to animal products, with bovine meat being the largest emitter. Emission data was visualized to highlight differences between categories.

Regression Models: Linear and decision tree regressors performed well in predicting emissions, as shown by low RMSE values.

Technologies Used

Python Libraries: Pandas, Scikit-learn, Pycountry, Matplotlib

Clustering Algorithms: K-means

Regression Models: RandomForest, DecisionTree, AdaBoost, Linear Regression

Project Structure

data/: Contains raw and cleaned datasets.

notebooks/: Jupyter notebooks used for exploratory data analysis and modeling.

src/: Python scripts for data cleaning, analysis, and modeling.

results/: Visualizations and clustering results.

README.md: Project overview and instructions.

Installation

Clone the repository:

git clone https://github.com/denizavukat/World-Food-Feed-Production.git

Create a virtual environment and activate it:

python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`

Install the required packages:

pip install -r requirements.txt

Usage

Run the Jupyter notebooks in the notebooks/ directory to explore data analysis and machine learning modeling.

Modify the scripts in src/ to try different clustering and regression techniques.

Results

Detailed results, visualizations, and discussions are available in the results/ directory.

Clustering results are visualized as maps to illustrate production similarities across countries.

License

This project is licensed under the MIT License.

Acknowledgements

Data sourced from Kaggle: Who Eats the Food We Grow? and Environmental Impact of Food Production.

