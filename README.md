# Coursera - Getting and Cleaning Data

One of the most exciting areas in all of data science right now is wearable computing. Companies like Fitbit, Nike, and Jawbone Up are racing to develop the most advanced algorithms to attract new users. The data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Here are the data for the project:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

## Setup:

1. Download and setup [RStudio](http://www.rstudio.com/).
 
2. Set your working directory.

3. Run run_analysis.R

4. File `UCI_HAR_tidy.csv` will be created

## Task:

R script `run_analysis.R` that does the following:

* Merges the training and the test sets (from the link above) to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names.
* From the data set in step 4, creates a second, independent tidy data set `UCI_HAR_tidy.csv` with the average of each variable for each activity and each subject.

## Codebook:

Check `codebook.md`