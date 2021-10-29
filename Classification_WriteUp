Abstract: 
The goal of this project is to use classification models to accurately predict whether an applicant should be approved for a loan. 

Design:
The data was gather from a Kaggle dataset. Classifying loan approvals accurately via modeling would minimize the amount of loan defaults the bank receives and there minimizing their overall loss. 

Data: 
The dataset contains over 100,000 data points and over 10 features. I pulled 15,000 rows out of 100,000 at random to begin my analysis. A few feature highlights include: total credit card limit, saving amount, is employed, yearly salary.  The features that were engineered include: available score, debt to income ratio, dependent status. 

Algorithm: 
Preprocessing: I started by loading the dataset obtained from Kaggle and pulling a sample of 15000 random rows to further analyze. I filled in the NAs with 0s and removed some of the outliers. I scaled all the features and did a train test split. I found a baseline model for KNN, Logistics Regression, and Random Forest with their optimal parameters. I also found a baseline precision score for Logistic Regression and Random Forest. These are the two models that I will be focusing on. The percent of the positive class is 45% and negative class is 54%, so I will not be addressing a class imbalance issue. 

Featuring Engineering: Created an available score feature where it adds a 1 if a loan requesters savings + checking amount is greater than their yearly average credit card debt. The available score feature slightly increased the precision score from the baseline models. Then I created a total debt to total income ratio feature with the total debt being the total credit card limit * the average percentage credit card limit used last year. Total Income is the savings amount + checking amount + yearly salary. The total debt to total income ratio slightly increased some of the scores except the Random Forest Precision Score, and the Logistics Regression and Random Forest AUC scores. Then I created the last feature engineer to be the dependent status. This is the yearly salary / number of dependents of the loan requester. If this value is greater than $12500 then that loan requester receives a 1 as the dependent status. $12500 is the average cost of a dependent in 2012 (when the data was pulled). The dependent status feature slightly increased some of the scores except the Random Forest Cross Validation Score and the Logistics Regression AUC score. After each feature engineer addition, I would re-standardize and re-split and re-cross validate all the features. I am mainly focusing on the Precision Score, CV Score, and AUC Score for both a Logistics Regression Model and Random Forest Model. 

Then I finally ran the algorithm through the test set and plotted the confusion matrix. I plotted the importance of each feature and analyzed the coefficients from the Logistics Regression model. 


Tools: 
Numpy and Pandas for data manipulation and EDA .
 Scikit-learn for modeling and interpreting. 
Matplotlib and Seaborn for visualizing. 

