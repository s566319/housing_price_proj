## Project: Housing Price Projection Project
## Author:  Inga Miller
## Date: November, 2024
## Email: S566319@nwmissouri.edu
## Institution: Northwest Missouri State University, Maryville MO 64468, USA

# Description: The project's domain is real estate.  It was chosen due to the high interest in the real estate pricing projection for investment possibilities. The data problem is the ability to predict if the market with go up or down, in turn will investors lose or gain the capital invested.


Keywords
Data Analytics
Data Visualization

# Table of Contents
Introduction
Goals of this Research
Data Overview and Collection
Data Descriptive Statistics
Data Types
Data Sources
Data Dictionary
Data Processing and Cleaning
Exploratory Data Analysis
Data Visualization
Data Trends
Model Training, Selection, and Evaluation
Results
Conclusion
Limitations of project
Ideas for future work
References

# Introduction
Real estate pricing projection has been a topic for investment possibilities. This project analyzes housing data in Washington state from May of 2014 to May of 2015.

# Goals of this Research
The goal of this research is to provide market trend analysis and predictions to investors as a decision making tool. It will be achieved by showing the final results of the model.

# Data Overview 
The data set used for this research comes from Kaggle, and includes values from May of 2014 to May of 2015, and lists property details such as price, number of bedrooms and bathrooms, the year it was built, the zip code of the property location, and very detailed information on the size of each property. The data set includes all the zip codes ranging from 98001 to 98199. The covered area is 28 miles long, stretching from Federal Way, WA to Seattle, WA.

# Data Processing and Cleaning
The initial dataset had 21613 rows and 21 columns. After removing several outliers, the cleaned data set was left with 21587 rows and 21 columns that are essential to this analysis.

# Data Attributes
The dataset includes the following key attributes:
Date: Date of the sale
Price: Price the property sold for
Bedrooms: Count of Bedrooms
Bathrooms: Count of Bathrooms
Condition: Condition rating of the property (ranging from 1 to 5)
Year built: Year the property was built
Zip code: Zip code where the property is located 

# Model Training, Selection, and Evaluation
The model training was started with data preparation.  The data was ensured to be cleaned, pre-processed, and then split into 80/20 ratio.  The data was split that way due to following the principle of the Pareto Principle (also known as the "80/20 rule") where 80 percent of the effect comes from 20 percent of the causes. The test size was 20 percent of the date or 4317 data points, while the training set was 80 percent or 17,269 rows of data.  By dedicating 80 percent of the data to training, the model has ample information to learn complex relationships within the data. 

After data preparation, a model selection step was performed where three separate models (Linear Regression Model, Random Forest Regressor, and Decision Tree Regressor) were trained. Each model was exposed to training data, allowing it to learn patterns and relationships. All three models were compared by looking at RMSE and R squared.

In model evaluation step, Decision Tree Regressor model was selected to predict future house prices. Model performance was deemed to be satisfactory; therefore, returning to model selection phase was not needed.

The following results are shown after the data is split between train and test sections: Training set shape: (17269, 5) (17269,)
Testing set shape: (4318, 5) (4318,)

# Conclusion
Overall, in five years, the National Association of Realtors (NAR) expect prices to have appreciated a total of 15 to 25 percent. This model predicts that 3 bedroom, 2 bathroom house built in 1951 in zip code 98125 will sell for 538,000 dollars in the future.
The results of the models are as follows:
![alt text](image-1.png)

The following pricing model was generated to predict pricing:
![alt text](image.png)

# Limitations of Project
The data is limited to the zip codes ranging from 98001 to 98199 in the 28 mile long covered area stretching from Federal Way, WA to Seattle, WA.  The future predictions will be limited to those zip codes.  The data is also limited to the years of the house sales. All of the data was collected for sales between May of 2014 to May of 2015, which eliminated any trend that could had occurred over the years. The model also predicts prices based on the five features specified: 'price', 'bedrooms', 'bathrooms', 'year built', and 'zip code'. Other features are not considered for this analysis.

# Ideas for Future Work
 Additional work on the model will enhance the predictions and increase the value for home buyers and investors. The additional work would include more zip codes across several states, and more data attributes would be analyzed. It would allow the potential home buyers more accurate analysis and investments.

Project Resources
Kaggle Dataset
GitHub Repository
Overleaf Project
Tableau Dashboard

Setup Instructions

Install JupyterLab:
pip install jupyterlab

Create / activate / install virtual environment with the following commands in a new terminal:
create:
python3 -m venv .venv

activate:
.venv\Scripts\activate

