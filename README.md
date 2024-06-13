# Predictive-Modeling-of-Health-Insurance-Charges-Analyzing-Demographic-and-Lifestyle-Factors


### SOURCE OF DATA SET
This project used the “Medical Cost Personal Dataset.” Available on Kaggle, it contains information about individual health insurance charges. 
The characteristics include age, sex, BMI, number of children, smoking habits, region, and insurance charges.
This dataset is a useful tool for examining the relationships between lifestyle and demographic characteristics. Considering both 
numeric (age, BMI, charges, number of children) and categorical (sex, smoking status, region) variables. This dataset offers an effective foundation for carrying out 
thorough studies and developing predictive models to comprehend and project medical insurance charges based on individual factors. Dataset can be accessed through the link 
below.
(https://www.kaggle.com/datasets/mirichoi0218/insurance/data)

### DATA PREPROCESSING
This project uses python for data cleaning. I imported my python library pandas as pd which help me to load my dataset.
My dataset contains 1338 rows × 7 columns. Firstly, an extensive check was performed on the dataset to identify duplicates and missing entries to maintain integrity of the 
data and avoid bias.
The data types were then evaluated to make sure they were consistent and compatible with the regression model.
Categorical variables such as 'sex', 'smoker', and 'region' were encoded into numerical format using label encoding techniques allowing their integration in
regression analysis. Binary categorical variables like 'smoker' and 'sex' (binary categorical variables) were encoded to 0s and 1s for analytical purpose.
In preparing the dataset for regression analysis, several critical steps such as data description, drop and correlation were taken to ensure data quality and suitability for
modeling purposes.
Now that the dataset has been cleaned and processed and contains only numerical values and encoded categorical values, it is prepared for model fitting and interpretation. 
This will allow me to use linear or multiple regression to examine the relationship between predictors
(such age, BMI, and smoking status etc) and the target variable (insurance charges).

### DISCUSSION ON HYPOTHESIS AND STATEMENT OF PROBLEM
- HYPOTHESIS 1
Analysing the data would aid Investigating the influence of several demographic factors (age, sex, region, and smoking status) on insurance charges.
Age and Sex on Insurance charges
It is important to know If there is a relationship between age and paying more insurance charges? The different health requirements may cause disparities in insurance charges and gender based. This can be achieved by knowing if there is statistical significance between age or sex.
Region and smoker on Insurance charges
Differences in healthcare provision across regions can impact insurance charges. This posit if there is a change in insurance charges in the region? For attribute smoker, smoking can cause various health issues potentially increasing insurance charges for smokers. This can ask the question if smokers' insurance charges differ significantly from one another?

This approach will not only improve comprehension of how each variable influences insurance on its own but also explain the impact. These findings are essential for administrators in healthcare planning, and individuals making informed decisions.
- HYPOTHESIS 2
The analysis will help predict the relationship between the number of children and Insurance charges. In families, healthcare expenses are a major financial concern. As the number of children increases there might be a relative increase in the amount of medical insurance and expenses. Examining the likelihood of children influences how much health insurance costs might be impacted. The investigation will help insurance firms make policy.
- HYPOTHESIS 3
  The analysis will help determine if BMI influences insurance charges. Higher BMI values are related to a variety of health hazards, which could result in higher healthcare costs. Having a good knowledge of how BMI affects insurance charges is germane for health providers to manage risk associated with health finance. This analysis helps insurance firms comprehend the financial effects of varying BMI levels.

  ### TECHNIQUES
This work utilises Regression analysis (Linear and Multiple) for exploring the dataset. The implementation of both linear regression and multiple regression approaches is essential in predicting insurance charges that impact upon lifestyle and demographic characteristics. It is suitable to use linear regression to examine the relationship between two continuous variables. A single predictor and dependent variable. It is uncomplicated and easy to interpret, making it appropriate for simple analysis.

A fundamental understanding of the direct influence of BMI or number of children is provided by linear regression. Considering that the dataset contains continuous variables like insurance charges number of children or BMI, linear regression is a good choice for determining the relationship between these characteristics. It makes it possible to evaluate the precise relationship between changes in insurance charges and variations in BMI or number of children, giving rise to an adequate understanding.

A linear regression model for BMI is shown below.
Y = a + bX
Where Y = Dependent variable (Insurance charges)
a = constant
b = coefficient
X = independent variable (BMI)
The same model can be adopted for the attribute number of children used in linear regression. However, multiple regression allows for a more thorough study by considering the combined impact of several characteristics. It enables a more thorough investigation of complex relationships and interactions between variables. Considering the variety of the dataset which includes several attributes which are age, smokers, sex, and region these variables are discrete in nature and are best handled by a multiple regression. Multiple regression can be used for both continuous and categorical dataset. This approach makes it possible to evaluate several factors at once, including
categorical variables. Hence the attribute was transformed to dummy variable for easier application in analysis.

### PROCESSING OF THE TECHNIQUES USING PYTHON
The model was processed with python. The linear regression model identifies the best-fitting line that minimizes the discrepancy between predicted and actual insurance charges depending on changes in X. Categorical variables were encoded for multiple regression. The model was fit for the Y and multiple predictors considering the effect on dependent variables. I evaluated two models using R squared to determine the proportion of variance in Y explained by X. Similarly, interpreting by coefficient, for positive coefficient in X, it will indicate an association in Y holding other variables constant.

### CONCLUSION
The techniques aid a well-informed recommendation, by exploring the dataset and stating the relationship and prediction. This will help inform stakeholders about healthcare planning and
insurance policy adjustments by gaining a thorough understanding of the complex relationships present in the information.
