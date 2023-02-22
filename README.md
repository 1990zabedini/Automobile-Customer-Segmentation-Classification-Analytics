# Automobile-Customer-Segmentation-Classification-Analytics
This is a multi-class classification problem regarding customer segmentation including 4 different segments (A, B, C, and D). There are 9 independent features and one dependent feature. The dataset shape is (8068,10) including numerical and nominal variables.
The first part is exploratory data analytics (EDA):
Handling missing values:
based on the EDA and finding out the elationship between different features and specifically the relationship between dependant and independant features, four different methods including mean,median and mode replacement, random sample creation, capturing the missing value importance by creating extra featues and missing value replacement based on the dependant-independant feature relationship were used. 
handling categorical feature:
based on the number of categories and the type of the nominal feature(categorical and ordinal), two different methods were used. one-hot-encoding creating dummy variables and also one-hot-encoding with feature having many different categories were used. 
handling outliers:
in this problem the outlier were not removed because it is a customer segmentation problem and abnormal patterns might identify imprtant unusuall customer behavior.
data scaling:
Rescaling data using standard scaling. Based on the experience standard scaling was used to rescale the data. it is important to not that in order to avoid data leakage, the train and test split was done befor data rescaling.
feature transformation:
as linear regression was one the model to used and the fact that linear regression has the hypothesis regarding features following normal distribution, numerical feature transformation was done using different techniques contains:
log
root square
reciprocal
exponential
boxcox
As the number of categories in Family_Size and Work_Experience are lower than 25, we could not consider these features as numerical features and did not apply feature transformation techniques on them.
feature selection:
Feature Selection methods like corelation and statistical tests were not applyed on the data as the number of feature are not huge
the models used in this problem were linear regression and also random forest.
the final accuracy (0.5258) and also other metrics reached acceptble scores compared to the similar work have been done on this dataset
