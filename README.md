#SCT_ML_1

#House Price Prediction using Linear Regression

##Project Overview

This project predicts house prices based on key property features such as the number of bedrooms, bathrooms, and total square footage.
Using a Linear Regression model, it explores how each of these features influences the overall price of a home.


##Objectives

* Clean and preprocess housing data
* Handle missing values effectively
* Train and evaluate a Linear Regression model
* Visualize relationships between variables and predicted outcomes
* Interpret coefficients to understand feature importance


##Tools & Libraries Used

* Python
* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn


##Data Preprocessing

* Checked for missing values and filled them using the median for numeric features and mode for categorical features.
* Selected key variables for training:

  * size (square footage)
  * beds (number of bedrooms)
  * baths (number of bathrooms)
* Target variable: price


##Model Training and Evaluation

The dataset was split into training (80%) and testing (20%) sets.
A Linear Regression model was trained on the training data and evaluated using Mean Squared Error (MSE) and R² Score.

Results:

* Mean Squared Error: 100,590,843,678.46
* R² Score: 0.656

Model Coefficients:

* size → +487.23
* beds → -102,010.08
* baths → +119,735.90
* Intercept → 111,259.57

##Insights

* The model explains about **65.6% of the variation in house prices.
* Square footage has the strongest positive effect on price.
* Bathrooms also increase price, while bedrooms show a small negative coefficient, possibly due to correlation with other variables.
* The Actual vs Predicted plot shows a mostly linear trend, indicating decent model performance.

##Visualizations

* Pairplot showing relationships between size, beds, baths, and price.
* Scatter plot comparing Actual vs Predicted Prices, visualizing model accuracy.

##How to Run the Project

1. Clone this repository to your local machine.
2. Navigate to the project folder.
3. Install the required Python libraries.
4. Open and run the Jupyter Notebook to view the analysis and results.

##Future Work

* Include additional features like location or ZIP code for higher accuracy.
* Convert lot size units for better consistency.
* Explore more advanced models such as Ridge, Lasso, Random Forest, or XGBoost.
* Build a simple web app using Flask or Streamlit for user interaction.

##Conclusion

This project demonstrates a complete machine learning workflow from data cleaning and feature selection to model evaluation and insight generation.
It serves as a solid foundation for anyone exploring regression modeling and predictive analytics in real estate.
