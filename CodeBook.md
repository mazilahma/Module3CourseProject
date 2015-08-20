##Data sets
Abstract: Human Activity Recognition database built from the recordings of 30
subjects performing activities of daily living (ADL) while carrying a waist-mounted
smartphone with embedded inertial sensors.

The datasets contains 6 activities: 
* WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING
* There are two folders: TEST and TRAIN
* There are 561-feature vector with time and frequency domain
* variables of activities described in the features.txt file
* Required to extract only the “mean” and “std” features
* The dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data

|DataSet Characteristics|Associated Tasks|Attribute Characteristics|Number of Instances|Date Donated| Missing Values|
|-----------------------|----------------|-------------------------|-------------------|------------|---------------|
|Multivariate,Time-Series| Classification,Clustering|  N/A         |561                |2012-12-10  | N/A           |
 
###Raw data set

The raw data set contains variables including:
* subject - An identifier of the subject who carried out the experiment.
* label - An activity label.
* accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ
* time domain signals (prefix 't' to denote time) 
* frequency domain signals (prefix 'f' to denote frequency)
* mean()
* std()

###Tidy data set

Tidy data set contains the same variables as the raw does, but the variables were renamed according to following rules:
* All lower case when possible
* Descriptive names  
* Not duplicated (the variable names are unique)
* Remove underscores or dots or white spaces(dashes and parentheses) 

###Variables in raw and tidy data set
|Raw data set 	           |   Tidy data set       |
|-------------------------|-----------------------|
|subject 	                |      subject          |
|label 	                  |   label               | 
|tBodyAcc-mean()-X 	      | tBodyAccMeanX         |
|tBodyAcc-mean()-Y 	      |   tBodyAccMeanY       |
|tBodyAcc-mean()-Z 	      |   tBodyAccMeanZ       |
|tBodyAcc-std()-X 	       |     tBodyAccStdX      |
|tBodyAcc-std()-Y 	       |     tBodyAccStdY      |
|tBodyAcc-std()-Z 	       |     tBodyAccStdZ      |
|tGravityAcc-mean()-X 	   |   tGravityAccMeanX    |
|tGravityAcc-mean()-Y 	   |   tGravityAccMeanY    |
|tGravityAcc-mean()-Z 	   |   tGravityAccMeanZ    |
|tGravityAcc-std()-X 	    |     tGravityAccStdX   |
|tGravityAcc-std()-Y 	    |     tGravityAccStdY   |
|tGravityAcc-std()-Z 	    |     tGravityAccStdZ   |
|tBodyAccJerk-mean()-X 	  |    tBodyAccJerkMeanX  |
|tBodyAccJerk-mean()-Y 	  |    tBodyAccJerkMeanY  |
|tBodyAccJerk-mean()-Z 	  |    tBodyAccJerkMeanZ  |
|tBodyAccJerk-std()-X 	   |   tBodyAccJerkStdX    |
|tBodyAccJerk-std()-Y 	   |   tBodyAccJerkStdY    |
|tBodyAccJerk-std()-Z 	   |   tBodyAccJerkStdZ    |
|tBodyGyro-mean()-X 	     |    tBodyGyroMeanX     |
|tBodyGyro-mean()-Y 	     |    tBodyGyroMeanY     |
|tBodyGyro-mean()-Z 	     |    tBodyGyroMeanZ     |
|tBodyGyro-std()-X 	      |   tBodyGyroStdX       |
|tBodyGyro-std()-Y 	      |   tBodyGyrStdY        |
|tGravityAccMag-std() 	   |   tGravityAccMagStd   |
|tBodyAccJerkMag-mean() 	 |tBodyAccJerkMagMean    |
|tBodyAccJerkMag-std() 	  |tBodyAccJerkMagStd     |
|tBodyGyroMag-mean() 	    |tBodyGyroMagMean       |
|tBodyGyroMag-std() 	     |tBodyGyroMagStd        |
|tBodyGyroJerkMag-mean()  |tBodyGyroJerkMagMean   |
|tBodyGyroJerkMag-std() 	 |tBodyGyroJerkMagStd    |
|fBodyAcc-mean()-X 	      |   fBodyAccMeanX       |
|fBodyAcc-mean()-Y 	      |   fBodyAccMeanY       |
|fBodyAcc-mean()-Z 	      |   fBodyAccMeanZ       |
|fBodyAcc-std()-X 	       |     fBodyAccStdX      |
|fBodyAcc-std()-Y 	       |     fBodyAccStdY      |
|fBodyAcc-std()-Z 	       |     fBodyAccStdZ      |
|fBodyAccJerk-mean()-X 	  |    fBodyAccJerkMeanX  |
|fBodyAccJerk-mean()-Y 	  |    fBodyAccJerkMeanY  | 
|fBodyAccJerk-mean()-Z 	  |    fBodyAccJerkMeanZ  |
|fBodyAccJerk-std()-X 	   |   fBodyAccJerkStdX    |
|fBodyAccJerk-std()-Y 	   |   fBodyAccJerkStdY    |
|fBodyAccJerk-std()-Z     |   fBodyAccJerkStdZ    |
|fBodyGyro-mean()-X 	     |    fBodyGyroMeanX     |
|fBodyGyro-mean()-Y 	     |   fBodyGyroMeanY      |
|fBodyGyro-mean()-Z 	     |   fBodyGyroMeanZ      |
|fBodyGyro-std()-X 	      |  fBodyGyroStdX        |
|fBodyGyro-std()-Y 	      |  fBodyGyroStdY        |
|fBodyGyro-std()-Z 	      |  fBodyGyroStdZ        |
|fBodyAccMag-mean() 	     |   fBodyAccMagMean     |
|fBodyAccMag-std() 	      |  fBodyAccMagStd       |
|fBodyBodyAccJerkMag-mean()| 	fBodyAccJerkMagMean |
|fBodyBodyAccJerkMag-std() | fBodyAccJerkMagStd   |
|fBodyBodyGyroMag-mean() 	 |  fBodyGyroMagMean    |
|fBodyBodyGyroMag-std() 	  |    fBodyGyroMagStd   |
|fBodyBodyGyroJerkMag-mean()|fBodyGyroJerkMagMean |
|fBodyBodyGyroJerkMag-std() |fBodyGyroJerkMagStd  |
