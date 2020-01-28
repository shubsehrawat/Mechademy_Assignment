# Mechademy_Assignment

# About Expander_Data Regression Analysis
  The function is created that takes the dataset as input and provide the Regression RMSE values using algorithms like Random Forest, 
  Decision Tree, Lasso Regression etc.
    1. The fist step is to treat the missing values in the dataset.
        i.The columns which have the percentage of missing values greater than 70%, those columns are dropped from the dataset as these 
        columns do not have any significat effect over the target variabes.
        ii.The columns which have the percentage of missing values less than 5%, the null values in these columns are removed.
        iii.The columns with percentage of missing values beyween 5% to 70%, then these columns are saperated into to categrories based on 
        the data-type of the columns. The null values of columns with object datatype are filled with the help of the "ffill" method and 
        the null values of the colunns with int of float type are filled with median values of that column.
    2. The next step is to split the "Timestamp" column into "Year","Month","Day","Hour","Min" columns saperately.
    3. After splitting the TimeStamp column, the next step is to do the outlier analysis. Plot the boxplot of each column , as it helps 
         in outlier detection. The outlier data is removed with the IQR Analysis
    4. The next stpe is to do the MIN_MAX Scaling of the dataset.
    5. Implementation of the Machine Learning Algorithms :
        Value of RMSE with "Decision Tree" :  1.8688808026920043 /////
        Value of RMSE with "Randon Forest Classifier" :  1.3815592463986823 /////
        Value of RMSE with "Linear Regression" :  2.205428729243894 /////
        Value of RMSE with "Ridge Regression" :  2.2054305825835407 /////
        Value of RMSE with "Rasso Regression" :  6.605390630958027 /////
        Value of RMSE with "Elastic Net Regression" :  39.803686717662345 /////
            
  
