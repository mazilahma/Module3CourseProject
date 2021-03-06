# Module3CourseProject
This course project is to demonstrate ability to collect, work with, and clean a data set.

The script contains a function sdata.analysis() that performs the following tasks:

***Test dataset***
* The test datasets is stored in the TEST folder
* It consists of the subject_test.txt, X_test.txt and y_test.txt files
* Read all 3 files
* Label X_test columns according to the features.txt
* Select only “mean” and “std” features from X_test
* Label Y_test column as “Activity ID” and “Activity Label”
* Label Subject_test column as “Subject”
* Combine all three into one dataset

***Training Dataset***
* The training datasets is stored in the TRAIN folder
* It consists of the subject_train.txt, X_train.txt and y_train.txt files
* Read all 3 files
* Label X_train columns according to the features.txt
* Select only “mean” and “std” features from X_train
* Label Y_train column as “Activity ID” and “Activity Label”
* Label Subject_train column as “Subject”
* Combine all three into one dataset

***Tidy Dataset***
* Combine the test and train datasets into one
* Write the output to a file “tidy_data.txt” file with write.table() using row.name=FALSE

To invoke the above function, please follow the steps below:
* set the current working directory by using setwd() function
* Copy run_analysis.R into the current working directory
* Ensure all samsung data is in the current working directory
```
Setwd('..') # specify the working directory 
source('run_analysis.R') # download samsung data in zip file and unzip it
sdata.analysis() # invoke the function to read test.data, train.data, features data
```

