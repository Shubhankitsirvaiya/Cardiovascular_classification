The dataset consists of data from an cardiovascular study done on the residents of town of Farmingham, 
Masachusettes. Our goal was to implement various Machine Learning models to predict whether the 
patient has a 10-year risk of future coronary heart disease. 
The dataset contains features such as: Sex, Age, behavioral information related to smoking, medical 
history information and current medical information pertaining to BP, prevalent stroke, Hypertension, 
Cholesterol levels, BP, Diabetes indicator, glucose levels, and the target variable – whether the patient 
has risk of coronary heart disease.
The approach we followed:
• Data Understanding
• EDA
• Data Preprocessing
• Building Models
• Choosing the best Model based on the appropriate evaluation metric for our problem statement
The data we were given mostly contained medical data about patients. The data provided was structured 
and in a tabular format. Our first step was to understand each of the features, exploring the permissible 
values each of these features can take, and understanding the impact of having a risk of coronary heart 
disease. 
We performed univariate and bivariate analysis on the data to understand their distributions and 
relationship with the target variable. We saw that the data has a class imbalance. We also performed 
multivariate analysis to check for correlations between the features, and the target variable.
Our next step was to preprocess the data. Here we performed missing value imputation, applied 
transformation to reduce skewness in the data, and applied binning on features. We also used SMOTE, 
and assigned class weights to treat the class imbalance. 
We chose recall as our evaluation metric to focus more on. Recall gives us the sensitivity. If we classify a 
person who has risk of heart disease wrongly, this will have higher implications as opposed to 
misclassifying a patient who does not have the risk. 
We built various models like – Decision Trees, Logistic Regression, Support Vector Machine, Random 
Forest and XGBoost. 
We performed cross validation and hyper parameter tuning and each of these models. XGBoost gave us 
the best recall score. However, with SMOTE, we were not able to increase our recall more. Using class 
weights, we got a better recall score. Using class weights, or using SMOTE, XGBoost model performed 
better than the other models. 
