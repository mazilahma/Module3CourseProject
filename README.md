# Module3CourseProject
A project to demonstrate ability to collect, work with, and clean a data set.

Script

The script contains a function run.analysis() that performs the actual job:

    reads train and test data sets and merges them
    processes the merged data set (extract the relevant variables, adds descriptive activity names, etc.)
    writes the merged data set to rawdata.csv
    generates the tidy data set
    writes the tidy data set to tidydata.csv
    returns the tidy data set

If you've a Samsung data available in the current directory, just run:

source('./run_analysis.R')
run.analysis() # invoke the actual function

Otherwise, you can use download.data() function provided in the script. The function will download the data archive and extract it. After that you can run run.analysis(). The full code:

source('./run_analysis.R')
download.data() # download samsung data and unzip it
run.analysis() # invoke the actual function

If you don't want to use download.data(), you should download the samsung data manually, unzip it in the current directory and then run:

source('./run_analysis.R')
run.analysis() # invoke the actual function

Note: In all the examples above, I assume that the script file run_analysis.R resides in the current working directory. If it does not, you should provide the correct path to the file to source it.
