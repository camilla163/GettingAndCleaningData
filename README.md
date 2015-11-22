# GettingAndCleaningData
Assignment for Coursera: Getting and Cleaning Data
##Load and Read Data
Loads training and test data files by name
Reads the files using read.table
Uses cbind() to merge subject and activity labels with samsung variable data
Uses rbind() to merge training data to test data, named all.data
##Label Variable Names to Merged Dataset
Uses the "features.txt" to label the samsung variable data with names()
Added ActivityCode and SubjectLabel prior to var.names so that columns would line up properly
##Convert Coded Activity Labels to Readable Activity Names
Use list indexing to make activity.label match up to the new column ActivityLabel
##Extract mean and stdev for each measurement
Uses grep() and colnames() to find variable names with 'mean' and 'std' in column name
Assign subsetted data to subset.cols and make new dataframe called all.summary.data
##Create a Second Tidy Dataset of the average of each variable for each subject and each activity
Use all.summary.data 

