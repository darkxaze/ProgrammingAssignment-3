Analysis Flowchart
-----------------

### 1. Read and merge data in files

The following are: labelling files: activity\ labels.txt and features.txt: subject\ test.txt, X\ test.txt (assigning names to columns with feature names) and y\ test.txt
- test information: subject\ train.txt, X\ train(txt) and y\ train.txt (assign column names to function names).
- merge all training files into one training data horizontally - merge all trial files into single test data horizontally - merge training and vertically test data into one single data -

###2. Only extract the medium and standard measurement deviation

- maintain the Id subject and actvitiy columns - identify 'mean' or 'std' column names.

### 3. Use descriptive activity names to name the activities in the data set

-   change the activity column from numberse 1-6 to descriptive activities: WALKING, WALKING\_UPSTAIRS, WALKING\_DOWNSTAIRS, SITTING, STANDING, LAYING

### 4. Label the data set with descriptive variable names

-   remove the () in the columns to make the variable names cleaner and easier to read
-   for a description of the variables, please refer to 'FEATURE VARIABLES' below

### 5. Create a second, independent tidy data set with the average of each variable for each activity and each subject


Feature engineering

The features of this database come from the three-axis raw signals tAcc-XYZ and tGyro-XYZ accelerometer and gyroscope. The time domain signals were captured with a constant rate of 50 Hz (prefixed 't' to denote time). The median filters and a low pass butterworth filter for the 3rd order with an angle frequency of 20 Hz were then filtering for noise deletion. In the same manner, the acceleration signal was separated by another low pass Butterworth filter with a corner frequency of about 0.3 Hz in body and gravity accelerations signals (tBodyAcc-XYZ and tGravityAcc-XYZ).

The linear body acceleration and angular speed were subsequently derived on time for Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). The magnitude was also calculated using the Euklidean standard for these three-dimensional signals (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).

In some of the signals fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyro-XYZ were finished with Fast Fourier Transform (FFT). (Note 'f' for signalling the domain of frequencies).

These signals were used to estimate variables of the feature vector for each pattern:
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.

feature variables

Time signals

-   tBodyAcc-XYZ
-   tGravityAcc-XYZ
-   tBodyAccJerk-XYZ
-   tBodyGyro-XYZ
-   tBodyGyroJerk-XYZ
-   tBodyAccMag
-   tGravityAccMag
-   tBodyAccJerkMag
-   tBodyGyroMag
-   tBodyGyroJerkMag

Frequency domain signals

-   fBodyAcc-XYZ
-   fBodyAccJerk-XYZ
-   fBodyGyro-XYZ
-   fBodyAccMag
-   fBodyAccJerkMag
-   fBodyGyroMag
-   fBodyGyroJerkMag

The set of variables that were estimated from these signals are as follows:

-   mean: Mean value
-   std: Standard deviation

