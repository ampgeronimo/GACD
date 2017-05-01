#Code Book

This document describes the code inside run_analysis.R.

The code is splitted (by comments) in some sections:

Downloading and loading data
Manipulating data
Data

#Downloading and Loading data

Reads the descriptive activity names to activity_labels
Reads the column names of data to features
Reads the X_test data frame to x_test
Reads the y_test data frame to y_test
Reads the X_train data frame to x_train
Reads the y_train data frame to y_train
Reads the subject_test data frame to subject_test
Reads the subject_train data.frame to subject_train

#Manipulating Data
1. merging subject_test,y_test,x_test, subject_train,y_train,x_train into one data frame df
2. renaming headers using features data frame
3. changing data in activity column to descriptive activity names using activity_labels data frame
4. subsetting columns with column names containing strings "mean()" or "std()"
5. reshaping data to skinny format
6. output data

#Data
id 
  id number of the subject
    01...30
  
activity
  label of the activity
    WALKING
    WALKING_UPSTAIRS
    WALKING_DOWNSTAIRS
    SITTING
    STANDING
    LAYING
  
variable
  kind of variable which average values are calculated
    mean
    std

average
  the average of mean or std values
