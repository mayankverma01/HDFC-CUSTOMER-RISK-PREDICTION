Tool used : Python Jupyter Notebook

Step By Step Approach:
1 Import Data (Train And Test)
	*Define Hypothetical relation(Define Y & X variable)
2 Data Preparation
	*Remove row and columns which have all null values
	* Delete colums whose have more than 70 % missing value
	* Convert all the column(morethan 50% and less than 70% missing value) in 0 and 1
		0 -> Null cell
		1 -> not Null cell
	* Create Data Audit Report
		function that contain frequency detail of features.
	* Outlier treatment for continuous variable ant 99% quantile
	* Missing value treatment
		mean -> for continuous variable
		median-> for ordinal variable [1,2,3,4,5]
3 Factor Analysis
	* PCA (Principal Component analysis) for variable reduction.
		509 variable explain 99% Data
		81 variable explain 80% data
		loading result show equal value for most of the variable
	* find correlation matrix
		take columns which have less than 70 % correlation
			509 columns remain
	*Featur Engineering
	* XgBoost Classifier use for the feature extraction
		select 91 variable

4 Split Training data in Train and Test(as a Validation data) in 67- 33 ratio

5 Model Building on Training Data
	*use logistic Regression,Decision Tree, Random Forest, Ridge Classifier
6 Validate the model using testing data
	* Re-run the model
	*Scoring the Model,Confusion Matrix,
	*Prediction and Evaluation
	*Cross Validation
	*Outof all these Classifier accuracy of Random Forest is yery High. 
	 So we select Random Forest Classifier.	
	*f1-score ->86&
7 Result of Test Data
	*Re-run model on Giving test data
8 Preparing the final reports to share the result
	
	
	
	

	


