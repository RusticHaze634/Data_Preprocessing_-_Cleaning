# Data Preprocessing & Cleaning
Sample Data Preprocessing, Cleaning and Feature Engineering

### Presentation through a Project

## Project : House Prices- Advanced Regression Techniques
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
- Set ID coumn as Index
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
 
 ## Handling Missing Value of Dataset and BSMT Feature
 
 - Check for null values
 - Check for BSMT features and its missing values
 - Check for null values
 - Fill in with NAN values
 - Check shape of data
 - Create a bucket using range
 - Replace NAN value of BsmtFinType2 by mode 
 - 
   
