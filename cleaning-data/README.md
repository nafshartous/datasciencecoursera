Script
======


To run run_analysis.R

  -  open the script and set the variable 

        rootDir 

     to the path to the Dataset directory.  


  - Then load the script into R.


The script performs the following steps

1.    Merges the training and the test sets to create one data set by using rbind to combine the two data frames.
      
2.    Extracts only the measurements on the mean and standard deviation for each measurement. 
      Only the variables containing "mean" or "std" are extracted.  This is done by subsetting 
      to extract the relevant columns, and the combining the subsets using cbind.

3.    Uses the descriptive activity names to name the activities in the data set.  This is done
      by mapping function labelActivities over the integer values (1..30) representing the activities.

4.    Label the data set with descriptive variable names. 

5.    From the data set in step 4, a tidy data set is created by averaging each variable for each activity and each subject.
      This is done by applying the aggregate function.




Code Book 
=========

Activity                    Descriptive activity Label
Subject                     Id of the subject/person performing the activity

 The following measurements were taken using the embedded accelerometer and gyroscope of the (Samsung Galaxy S II)
 3-axial linear acceleration and 3-axial angular velocity were captured at a constant rate of 50Hz.

 Each of the following columns represents represent the average of the meaurements for the same feature 
 of the same subject performing the activity in a given row.  See Dataset/README.txt for further details.

tBodyAcc-mean-X
tBodyAcc-mean-Y
tBodyAcc-mean-Z
tBodyAcc-std-X
tBodyAcc-std-Y
tBodyAcc-std-Z
tGravityAcc-mean-X
tGravityAcc-mean-Y
tGravityAcc-mean-Z
tGravityAcc-std-X
tGravityAcc-std-Y
tGravityAcc-std-Z
tBodyAccJerk-mean-X
tBodyAccJerk-mean-Y
tBodyAccJerk-mean-Z
tBodyAccJerk-std-X
tBodyAccJerk-std-Y
tBodyAccJerk-std-Z
tBodyGyro-mean-X
tBodyGyro-mean-Y
tBodyGyro-mean-Z
tBodyGyro-std-X
tBodyGyro-std-Y
tBodyGyro-std-Z
tBodyGyroJerk-mean-X
tBodyGyroJerk-mean-Y
tBodyGyroJerk-mean-Z
tBodyGyroJerk-std-X
tBodyGyroJerk-std-Y
tBodyGyroJerk-std-Z
tBodyAccMag-mean
tBodyAccMag-std
tGravityAccMag-mean
tGravityAccMag-std
tBodyAccJerkMag-mean
tBodyAccJerkMag-std
tBodyGyroMag-mean
tBodyGyroMag-std
tBodyGyroJerkMag-mean
tBodyGyroJerkMag-std
fBodyAcc-mean-X
fBodyAcc-mean-Y
fBodyAcc-mean-Z
fBodyAcc-std-X
fBodyAcc-std-Y
fBodyAcc-std-Z
fBodyAccJerk-mean-X
fBodyAccJerk-mean-Y
fBodyAccJerk-mean-Z
fBodyAccJerk-std-X
fBodyAccJerk-std-Y
fBodyAccJerk-std-Z
fBodyGyro-mean-X
fBodyGyro-mean-Y
fBodyGyro-mean-Z
fBodyGyro-std-X
fBodyGyro-std-Y
fBodyGyro-std-Z
fBodyAccMag-mean
fBodyAccMag-std
fBodyBodyAccJerkMag-mean
fBodyBodyAccJerkMag-std
fBodyBodyGyroMag-mean
fBodyBodyGyroMag-std
fBodyBodyGyroJerkMag-mean
fBodyBodyGyroJerkMag-std






