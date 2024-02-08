# tipsy_regression
Building regression models to explore the relationship between wine price and its sales!🍷

# Table of Contents
- General Info
- Setup
- Usage
- Challenges
- Project Results 
- Future Data Exploration Ideas
- Acknowledgements
- Contact

# General Information
I’m uploading the code of the regression models I trained on wine data!💻🍷

The goal was to explore the correlation between wine price and wine rating to see if the former influences the latter. I extracted the data from the web and then built and trained a linear regression ML model and a random forest regressor to make predictions about wine rating given their price. I also want to support other coders who are wine lovers just like me and are willing to train their own regressor(s)!🗺️🔎👣

I used a red-wine dataset available on Kaggle, made up of 8666 datapoints. I then explored the data, cleansed it, analysed it, and built and trained the models. I then plotted the models and computed their metrics.

# Setup
First off, make sure you have conda🐍👀:

`conda create -n <replace-with-name-you-want> python=3.11`

`conda activate <replace-with-name-you-want>`

`pip install -r requirements.txt`

# Usage
Check out the `wine_sales_project.ipynb` file in my repo to see how I've processed the data, built and trained the models!


# Challenges
The main challenge was finding a good feature engineering solution to use to make the data available for model training. For this project, I filtered the data by the prices that are lower than 100. This removes outliers in the data, which allows us to find better signal in the data. 

# Project Results
First, I trained a simple linear regression model three times. I gradually filtered the data according to the price of the wine (i.e., initially it was under £500, then £250, up to £100). The relationship between the price variable and the rating variable is positive. The higher the price, the higher the rating. At higher prices, the rating and price are linearly related. As the price starts decreasing, it's less linearly related. At higher prices, the rate of change of the rating is relatively constant. As the price goes down, the rating seems to go down faster. This means that the linear model might not be the best option to use to fit this data.

So I then trained another model: a random forest regressor, to see if it could be a better way to fit our data. We've also added `Country` as one of the features. We've discovered that the random forest is giving us slightly better results! Yet, there's no significant improvement. 

# Future Data Exploration Ideas
We could try to train a different machine learning model which could fit this data better (e.g., decision trees🌳, K-nearest neighbours👪🏠, etc.). We could even experiment with different independent variables, rather than the price. For example, does the region of origin of the wine influence its rating?🌏🔎

# Acknowledgements
A massive thank you to Ward Haddadin for your support! Training my first linear regression model wouldn't have been possible if it wasn't for your words of encouragement!

# Contact
For any question, drop me a line at giorgiadt14@gmail.com and I'll be happy to help you out! Feel free to message me on [LinkedIn](https://www.linkedin.com/in/giorgia-dim/) too! Happy coding!💻