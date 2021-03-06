##**The Script**
The script run_analysis.R executes 5 steps required to deliver a tidy data set suitable for analysis.
    1. Merges the training and the test sets to create one data set.
    2. Extracts only the measurements on the mean and standard deviation for each measurement. 
    3. Uses descriptive activity names to name the activities in the data set
    4. Appropriately labels the data set with descriptive variable names. 
    5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each     subject.

##**The Data**
The raw data set is the Human Activity Recognition Using Smartphones Dataset for which there is a link posed in the README.md document of this repository. 

##**The Variables**
The raw data is read into R by use of variables test, test_y, test_subject, train, train_y, train_subject.  fullData, full_y, and full_subject merges the test and train variables together.
features contains the correct column headings for the fullData set and mean.std is a numeric vector that is used to select the columns within fullData that contain mean and standard deviation information.
allData combines fullData, full_y, and full_subject.
data_avg is the organized data for the tidy data set submission.
