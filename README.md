# Credit_Risk_Analysis



Overview:


-	The purpose of this analysis was to assess the credit risk of potential borrowers by evaluating data provided by LendingClub (a peer-to-peer lending services company). This was achieved by testing the accuracy of multiple models built with statistical data analysis and machine learning techniques.


-	This project includes 6 statistical concepts:
o	4 Sampling Techniques
  	Oversampling using the RandomOverSampler
  	Oversampling using the SMOTE
  	Undersampling using ClusterCentroids
  	A combinatorial approach of over and undersampling using SMOTEENN

o	2 Models that Reduce Bias
  	BalancedRandomForestClassifier
  	EasyEnsembleClassifier
  
  
  
Results:


-	The first oversampling approach leveraged the RandomOverSampler concept to resample the data to illustrate the minority class subset of data used in the logistic regression model to examine dichotomous outcome variables.
  o	The balanced accuracy score indicates the model is accurate 64.44% of the time.
  o	The precision score of the low-risk loans was 100%, while it was only 1% for the high-risk loans.
  o	The recall scores were somewhat consistent. Both the high and low-risk loans landed in the 60-70% range.
![image](https://user-images.githubusercontent.com/96176817/167279543-090261f4-cc2e-4938-a438-b8515f916271.png)
![image](https://user-images.githubusercontent.com/96176817/167279546-478a5119-4278-4a3a-a990-7f329edbd1f0.png)

-	The second oversampling approach leveraged the synthetic minority oversampling technique (SMOTE) to resample the data to illustrate the minority class subset of data used in the logistic regression model to examine dichotomous outcome variables.
  o	The balanced accuracy score indicates the model is accurate 63.70% of the time.
  o	The precision score of the low-risk loans was 100%, while it was only 1% for the high-risk loans.
  o	The recall scores were somewhat consistent. Both the high and low-risk loans landed in the 60-65% range.
![image](https://user-images.githubusercontent.com/96176817/167279558-1fb5d7ad-913c-401d-b326-ddc63e63f09a.png)
![image](https://user-images.githubusercontent.com/96176817/167279561-11052f5f-b0eb-4876-82b7-fae420df0fee.png)

-	The undersampling approach leveraged ClusterCentroids to resample the data to illustrate the minority class subset of data used in the logistic regression model to examine dichotomous outcome variables.
  o	The balanced accuracy score indicates the model is accurate 52.93% of the time.
  o	The precision score of the low-risk loans was 100%, while it was only 1% for the high-risk loans.
  o	The recall scores were somewhat consistent.
    	High-risk loans = 61.00%

    	Low-risk loans = 45.00%
![image](https://user-images.githubusercontent.com/96176817/167279576-d3837b91-358f-4145-ade8-6118d1d6f423.png)
![image](https://user-images.githubusercontent.com/96176817/167279578-bac3ac50-6f89-4714-92e6-48b20efd1d22.png)

-	The combined approach leveraged the SMOTEENN (SMOTE and Edited Nearest Neighbors (ENN) algorithms combined) to remove outliers and resample the data to be used in the logistic regression model to examine dichotomous outcome variables.
  o	The balanced accuracy score indicates the model is accurate 63.76% of the time.
  o	The precision score of the low-risk loans was 100%, while it was only 1% for the high-risk loans.
  o	The recall scores were somewhat consistent.
    	High-risk loans = 70.00%
    	Low-risk loans = 57.00%
![image](https://user-images.githubusercontent.com/96176817/167279587-ae561122-de9e-45b9-b54f-7f023836027c.png)
![image](https://user-images.githubusercontent.com/96176817/167279592-c38169e5-b0d0-4c7d-96cf-2ccb8c2603bf.png)

-	The first bias reducing model leveraged BalancedRandomForestClassifier to create decision trees used to assess the data.
  o	The balanced accuracy score indicates the model is accurate 78.77% of the time.
  o	The precision score of the low-risk loans was 100%, while it was only 4% for the high-risk loans.
  o	The recall scores were somewhat consistent.
    	High-risk loans = 67.00%
    	Low-risk loans = 91.00%
![image](https://user-images.githubusercontent.com/96176817/167279612-55465c29-00df-43b0-b60d-1140b267c1a6.png)
![image](https://user-images.githubusercontent.com/96176817/167279618-40b5db32-46d6-476d-b5bd-4698de03266b.png)
![image](https://user-images.githubusercontent.com/96176817/167279628-f36d15bd-7891-45fb-8aa4-c399d5c04e02.png)

-	The second bias reducing model leveraged EasyEnsembleClassifier to implement the concept of Adaptive boosting. This technique uses an error reduction process.
  o	The balanced accuracy score indicates the model is accurate 92.54% of the time.
  o	The precision score of the low-risk loans was 100%, while it was only 7% for the high-risk loans.
  o	The recall scores were very consistent. Both the high and low-risk loans landed in the 90-95% range.
![image](https://user-images.githubusercontent.com/96176817/167279643-661049a5-e785-4f2d-bbea-d7a8a7c3405c.png)
![image](https://user-images.githubusercontent.com/96176817/167279647-15911ea5-983b-47ba-ac17-cb32a4cf0c02.png)



Summary:


-	In conclusion, the models did not provide enough proof to justify using them. However, the EasyEnsembleClassifier model was the most accurate based on its balanced accuracy, precision, and recall scores.
