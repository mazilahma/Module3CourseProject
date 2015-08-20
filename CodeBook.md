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


|Data Set         |Associated Tasks: | Attribute      |Number of   |Date DOnated: | Missing Values: |
|Characteristics: |                  |Characteristics:|Attributes: |              |                 |
|-----------------|------------------|----------------|------------|--------------|-----------------|
|Multivariate,    | Classification,  |  N/A           |561         |2012-12-10    | N/A             |
|Time-Series      | Clustering       |                |            |              |                 |

###Raw data set

Totally, the raw data set contains 68 variables:

    *subject - An identifier of the subject who carried out the experiment.
    *label - An activity label.

Plus 66 filtered features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. The time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz and a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, 
fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

These signals were used to estimate variables of the feature vector for each pattern:
-XYZ is used to denote 3-axial signals in the X, Y and Z directions.

    tBodyAcc-XYZ
    tGravityAcc-XYZ
    tBodyAccJerk-XYZ
    tBodyGyro-XYZ
    tBodyGyroJerk-XYZ
    tBodyAccMag
    tGravityAccMag
    tBodyAccJerkMag
    tBodyGyroMag
    tBodyGyroJerkMag
    fBodyAcc-XYZ
    fBodyAccJerk-XYZ
    fBodyGyro-XYZ
    fBodyAccMag
    fBodyAccJerkMag
    fBodyGyroMag
    fBodyGyroJerkMag

The set of variables that were estimated from these signals are:

    mean(): Mean value
    std(): Standard deviation

###Tidy data set

Tidy data set contains the same variables as the raw does, but the variables were renamed according to following rules:

    All lower case when possible - the variables names were not converted to lower case, since it would make them unreadable. Instead, the variable names were converted to satisfy camlCase rule.
    Descriptive (Diagnosis versus Dx) - the variable names are descriptive, so nothing special should be done.
    Not duplicated - the variable names are unique, so again nothing special had to be done.
    Not have underscores or dots or white spaces - dashes and parentheses were removed from variable names.

###Variables in raw and tidy data set
|Raw data set 	           |   Tidy data set       |
|-------------------------|-----------------------|
|subject 	                     subject
label 	                     label
tBodyAcc-mean()-X 	         tBodyAccMeanX
tBodyAcc-mean()-Y 	         tBodyAccMeanY
tBodyAcc-mean()-Z 	         tBodyAccMeanZ
tBodyAcc-std()-X 	            tBodyAccStdX
tBodyAcc-std()-Y 	            tBodyAccStdY
tBodyAcc-std()-Z 	            tBodyAccStdZ
tGravityAcc-mean()-X 	      tGravityAccMeanX
tGravityAcc-mean()-Y 	      tGravityAccMeanY
tGravityAcc-mean()-Z 	      tGravityAccMeanZ
tGravityAcc-std()-X 	         tGravityAccStdX
tGravityAcc-std()-Y 	         tGravityAccStdY
tGravityAcc-std()-Z 	         tGravityAccStdZ
tBodyAccJerk-mean()-X 	      tBodyAccJerkMeanX
tBodyAccJerk-mean()-Y 	      tBodyAccJerkMeanY
tBodyAccJerk-mean()-Z 	      tBodyAccJerkMeanZ
tBodyAccJerk-std()-X 	      tBodyAccJerkStdX
tBodyAccJerk-std()-Y 	      tBodyAccJerkStdY
tBodyAccJerk-std()-Z 	      tBodyAccJerkStdZ
tBodyGyro-mean()-X 	         tBodyGyroMeanX
tBodyGyro-mean()-Y 	         tBodyGyroMeanY
tBodyGyro-mean()-Z 	         tBodyGyroMeanZ
tBodyGyro-std()-X 	         tBodyGyroStdX
tBodyGyro-std()-Y 	         tBodyGyroStdY
tBodyGyro-std()-Z 	         tBodyGyroStdZ
tBodyGyroJerk-mean()-X     	tBodyGyroJerkMeanX
tBodyGyroJerk-mean()-Y 	      tBodyGyroJerkMeanY
tBodyGyroJerk-mean()-Z 	      tBodyGyroJerkMeanZ
tBodyGyroJerk-std()-X 	      tBodyGyroJerkStdX
tBodyGyroJerk-std()-Y 	      tBodyGyroJerkStdY
tBodyGyroJerk-std()-Z 	      tBodyGyroJerkStdZ
tBodyAccMag-mean() 	         tBodyAccMagMean
tBodyAccMag-std() 	         tBodyAccMagStd
tGravityAccMag-mean() 	      tGravityAccMagMean
tGravityAccMag-std() 	      tGravityAccMagStd
tBodyAccJerkMag-mean() 	      tBodyAccJerkMagMean
tBodyAccJerkMag-std() 	      tBodyAccJerkMagStd
tBodyGyroMag-mean() 	         tBodyGyroMagMean
tBodyGyroMag-std() 	         tBodyGyroMagStd
tBodyGyroJerkMag-mean()       tBodyGyroJerkMagMean
tBodyGyroJerkMag-std() 	      tBodyGyroJerkMagStd
fBodyAcc-mean()-X 	         fBodyAccMeanX
fBodyAcc-mean()-Y 	         fBodyAccMeanY
fBodyAcc-mean()-Z 	         fBodyAccMeanZ
fBodyAcc-std()-X 	            fBodyAccStdX
fBodyAcc-std()-Y 	            fBodyAccStdY
fBodyAcc-std()-Z 	            fBodyAccStdZ
fBodyAccJerk-mean()-X 	      fBodyAccJerkMeanX
fBodyAccJerk-mean()-Y 	      fBodyAccJerkMeanY
fBodyAccJerk-mean()-Z 	      fBodyAccJerkMeanZ
fBodyAccJerk-std()-X 	      fBodyAccJerkStdX
fBodyAccJerk-std()-Y 	      fBodyAccJerkStdY
fBodyAccJerk-std()-Z 	      fBodyAccJerkStdZ
fBodyGyro-mean()-X 	         fBodyGyroMeanX
fBodyGyro-mean()-Y 	         fBodyGyroMeanY
fBodyGyro-mean()-Z 	         fBodyGyroMeanZ
fBodyGyro-std()-X 	         fBodyGyroStdX
fBodyGyro-std()-Y 	         fBodyGyroStdY
fBodyGyro-std()-Z 	         fBodyGyroStdZ
fBodyAccMag-mean() 	         fBodyAccMagMean
fBodyAccMag-std() 	         fBodyAccMagStd
fBodyBodyAccJerkMag-mean() 	fBodyAccJerkMagMean
fBodyBodyAccJerkMag-std() 	   fBodyAccJerkMagStd
fBodyBodyGyroMag-mean() 	   fBodyGyroMagMean
fBodyBodyGyroMag-std() 	      fBodyGyroMagStd
fBodyBodyGyroJerkMag-mean() 	fBodyGyroJerkMagMean
fBodyBodyGyroJerkMag-std() 	fBodyGyroJerkMagStd
