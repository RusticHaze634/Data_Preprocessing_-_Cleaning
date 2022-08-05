# Data Preprocessing & Cleaning
Sample Data Preprocessing, Cleaning and Feature Engineering

### Presentation through a Project

## Project 1: House Prices- Advanced Regression Techniques
- **Objective** : _Predict the sales price for each house. For each Id in the test set, one must predict the value of the SalePrice variable._ 

### Libraries Used 
- NUMPY, pandas, Matplotlib.pyplot, Seaborn

## Dataset
- train.csv - the training set
- test.csv - the test set

**SOLUTION:**

## Data Concatination
- Training and testing dataset merging

## Exploratory Data Analysis (EDA) 
- Check the all data columns and their details
- Set ID column as Index
- **Show the null values using heatmap**
![attachment:heatmap.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/heatmap.png)

- Get the percentages of null value
- **Drop Columns** - If the null value % 20 or > 20, Ir has to be dropped
- Find the unique value count and unique value for each column
- **Describe the target**  
   Plot the Distribution of Target
 ![attachment:distplot.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/distplot.png)
 
 - **Generation of Correlation among data columns (Heatmap)**
 ![attachment:corelation.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/corelation.png)
 
 - **Modified Correlation Heatmap for Highly Correlated Features with SalePrice**
 ![attachment:correlationsalprice.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/correlationsalprice.png)
 
 - Plot regplot to get the nature of highly correlated data
 ![attachment:regplot.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/regplot.png)
 
 ## Handling Missing Value of Dataset and BSMT, Garage Feature
 
 - Check for null values
 - Check for **BSMT and Garage** features and its missing values
 - Check for null values
 - Fill in with NAN values
 - Check shape of data
 - Create a bucket using range
 - Replace NAN value of BsmtFinType2 by mode 
 - **Handling missing value of remaining features**
 - Check for Unique and Nulll values of other features
 - Use Fillna to replace null values
 - Handling missing value of **LotFrontage** feature
 
 ## Feature Transformation
 - Convert columns in str which have categorical nature but in int64
 - Convert a time related feature in month abbrevation
 - Creating a list for modified columns
 
 ## Convert categorical codes into order
 - Define Data Categories
 - Catinate the category codes columnwise
 - Keep unique value columns (Columns with few varieties of value)

### Show skewness of features 
- Use Distplot
![attachment:distplot2.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/distplot2.png)

- Decrease the skewnwnes of the data

## Dummy Variables
- Get object feature to convert in numeric using dummy variable
- Select and drop the dummy variables

## Scale Dataset
- Check Shape of modified data
- Scale dataset with robust scaler


## Machine Learning Model Building
- Check length of Training dataset
- Apply **k-fold Cross Validation** to get the correct patterns from the data

## Models applied 
- Linear Regression
- Support Vector Machine
- Decision Tree Regressor
- Random Forest Regressor
- Bagging & boosting
- XGBoost

## Hyperparameter Tuning 
- RandomizedSearchCV, GridSearchCV for SVM model
- XGBRegressor for XGBoost


## Feature Engineering / Selection to improve accuracy
- **Correlation Barplot for feature Engineering**

![attachment:corelationfeature.png](https://github.com/RusticHaze634/Data_Preprocessing_-_Cleaning/blob/main/Images/corelationfeature.png)

- **Drop features** those are not required  
**'YrSold',
 'LowQualFinSF',
 'MiscVal',
 'BsmtHalfBath',
 'BsmtFinSF2',
 '3SsnPorch',
 'MoSold'**
 
 **Run models again after Feature Engineering and Hyperparameter Tuning**
 
 ## Saving the Model
 - Us **'Pickle'** to save the model
 - Use the data 'model_house_price_prediction.csv'

## Result
- **Support Vector Machine with Accuracy** = **90%**
 
   
