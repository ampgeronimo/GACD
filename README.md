# GACD
Getting and Cleaning Data Project

load libraries (plyr, dplyr, and tidyr)

read all files:
- 'features.txt': List of all features.
- 'activity_labels.txt': Links the class labels with their activity name.
- 'train/X_train.txt': Training set.
- 'train/y_train.txt': Training labels.
- 'test/X_test.txt': Test set.
- 'test/y_test.txt': Test labels.
- 'subject_train.txt': Test subject ID.
- 'subject_test.txt': Train subject ID.

merge subject_test,y_test,x_test
merge subject_train,y_train,x_train

merge both tables

rename column headers

change data in activity column to descriptive activity names using activity_labels.txt

subset columns with column names containing mean() and std()

reshape data to skinny format

output data
