# Human Activity Recognition Using Smartphones Dataset

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

For full desciption of data open this link:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

# Features

Script `run_analysis.R` will produce file `UCI_HAR_tidy.csv` that contains the following features:

``` [1] "subject"                        
                
[2] "timeBodyAccelerometerMeanX"                     

[3] "timeBodyAccelerometerMeanY"                     

[4] "timeBodyAccelerometerMeanZ"                     

[5] "timeBodyAccelerometerStdX"                      

[6] "timeBodyAccelerometerStdY"                      

[7] "timeBodyAccelerometerStdZ"                      

[8] "timeGravityAccelerometerMeanX"                  

[9] "timeGravityAccelerometerMeanY"                  

[10] "timeGravityAccelerometerMeanZ"                  

[11] "timeGravityAccelerometerStdX"                   

[12] "timeGravityAccelerometerStdY"                   

[13] "timeGravityAccelerometerStdZ"                   

[14] "timeBodyAccelerometerJerkMeanX"                 

[15] "timeBodyAccelerometerJerkMeanY"                 

[16] "timeBodyAccelerometerJerkMeanZ"                 

[17] "timeBodyAccelerometerJerkStdX"                  

[18] "timeBodyAccelerometerJerkStdY"                  

[19] "timeBodyAccelerometerJerkStdZ"                  

[20] "timeBodyGyroscopeMeanX"                         

[21] "timeBodyGyroscopeMeanY"                         

[22] "timeBodyGyroscopeMeanZ"                         

[23] "timeBodyGyroscopeStdX"                          

[24] "timeBodyGyroscopeStdY"                          

[25] "timeBodyGyroscopeStdZ"                          

[26] "timeBodyGyroscopeJerkMeanX"                     

[27] "timeBodyGyroscopeJerkMeanY"                     

[28] "timeBodyGyroscopeJerkMeanZ"                     

[29] "timeBodyGyroscopeJerkStdX"                      

[30] "timeBodyGyroscopeJerkStdY"                      

[31] "timeBodyGyroscopeJerkStdZ"                      

[32] "timeBodyAccelerometerMagnitudeMean"             

[33] "timeBodyAccelerometerMagnitudeStd"              

[34] "timeGravityAccelerometerMagnitudeMean"          

[35] "timeGravityAccelerometerMagnitudeStd"           

[36] "timeBodyAccelerometerJerkMagnitudeMean"         

[37] "timeBodyAccelerometerJerkMagnitudeStd"          

[38] "timeBodyGyroscopeMagnitudeMean"                 

[39] "timeBodyGyroscopeMagnitudeStd"                  

[40] "timeBodyGyroscopeJerkMagnitudeMean"             

[41] "timeBodyGyroscopeJerkMagnitudeStd"              

[42] "frequencyBodyAccelerometerMeanX"                

[43] "frequencyBodyAccelerometerMeanY"                

[44] "frequencyBodyAccelerometerMeanZ"                

[45] "frequencyBodyAccelerometerStdX"                 

[46] "frequencyBodyAccelerometerStdY"                 

[47] "frequencyBodyAccelerometerStdZ"                 

[48] "frequencyBodyAccelerometerJerkMeanX"            

[49] "frequencyBodyAccelerometerJerkMeanY"            

[50] "frequencyBodyAccelerometerJerkMeanZ"            

[51] "frequencyBodyAccelerometerJerkStdX"             

[52] "frequencyBodyAccelerometerJerkStdY"             

[53] "frequencyBodyAccelerometerJerkStdZ"             

[54] "frequencyBodyGyroscopeMeanX"                    

[55] "frequencyBodyGyroscopeMeanY"                    

[56] "frequencyBodyGyroscopeMeanZ"                    

[57] "frequencyBodyGyroscopeStdX"                     

[58] "frequencyBodyGyroscopeStdY"                     

[59] "frequencyBodyGyroscopeStdZ"                     

[60] "frequencyBodyAccelerometerMagnitudeMean"        

[61] "frequencyBodyAccelerometerMagnitudeStd"         

[62] "frequencyBodyBodyAccelerometerJerkMagnitudeMean"

[63] "frequencyBodyBodyAccelerometerJerkMagnitudeStd" 

[64] "frequencyBodyBodyGyroscopeMagnitudeMean"        

[65] "frequencyBodyBodyGyroscopeMagnitudeStd"         

[66] "frequencyBodyBodyGyroscopeJerkMagnitudeMean"    
[67] "frequencyBodyBodyGyroscopeJerkMagnitudeStd"     

[68] "activity"     ```      

`subject [1]` - integer identifier of person who performed the activity for each window sample. Its range is from 1 to 30. 

`activity [68]` - activity performed by subject: `WALKING`, `WALKING_UPSTAIRS`, `WALKING_DOWNSTAIRS`, `SITTING`, `STANDING`, `LAYING`

Other features were made using original features from source data set

# Original Features

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag). 

Finally a Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals). 

The set of variables that were estimated from these signals are: 
* mean(): Mean value
* std(): Standard deviation

Features are normalized and bounded within [-1,1].

The acceleration signal from the smartphone accelerometer X,Y,Z axis in standard gravity units 'g'.

The body acceleration signal obtained by subtracting the gravity from the total acceleration. 

# Transformation to original features

Original features were transformed to a new set of features:

|Original features|Transformed features|
|-----------------|--------------------|
| tBodyAcc mean,std XYZ | timeBodyAccelerometerMean XYZ [2,3,4], timeBodyAccelerometerStd XYZ [5,6,7] |
| tGravityAcc mean,std XYZ | timeGravityAccelerometerMean XYZ [8,9,10], timeGravityAccelerometerStd XYZ [11,12,13] |
| tBodyAccJerk mean,std XYZ | timeBodyAccelerometerJerkMean XYZ [14,15,16], timeBodyAccelerometerJerkStd XYZ [17,18,19] |
| tBodyGyro mean,std XYZ | timeBodyGyroscopeMean XYZ [20,21,22], timeBodyGyroscopeStd XYZ [23,24,25] |
| tBodyGyroJerk mean,std XYZ | timeBodyGyroscopeJerkMean XYZ [26,27,28], timeBodyGyroscopeJerkStd XYZ [29,30,31] |
| tBodyAccMag mean,std | timeBodyAccelerometerMagnitudeMean [32], timeBodyAccelerometerMagnitudeStd [33] |
| tGravityAccMag mean,std | timeGravityAccelerometerMagnitudeMean [34], timeGravityAccelerometerMagnitudeStd [35] |
| tBodyAccJerkMag mean,std | timeBodyAccelerometerJerkMagnitudeMean [36], timeBodyAccelerometerJerkMagnitudeStd [37] |
| tBodyGyroMag mean,std | timeBodyGyroscopeMagnitudeMean [38], timeBodyGyroscopeMagnitudeStd [39] |
| tBodyGyroJerkMag mean,std | timeBodyGyroscopeJerkMagnitudeMean [40], timeBodyGyroscopeJerkMagnitudeStd [41] |
| fBodyAcc mean,std XYZ | frequencyBodyAccelerometerMean XYZ [42,43,44], frequencyBodyAccelerometerStd XYZ [45,46,47] |
| fBodyAccJerk mean,std XYZ | frequencyBodyAccelerometerJerkMean XYZ [48,49,50], frequencyBodyAccelerometerJerkStd XYZ [51,52,53] |
| fBodyGyro mean,std XYZ | frequencyBodyGyroscopeMean XYZ [54,55,56], frequencyBodyGyroscopeStd [57,58,59] |
| fBodyAccMag mean,std | frequencyBodyAccelerometerMagnitudeMean [60], frequencyBodyAccelerometerMagnitudeStd [61] |
| fBodyBodyAccJerkMag mean,std | frequencyBodyBodyAccelerometerJerkMagnitudeMean [62], frequencyBodyBodyAccelerometerJerkMagnitudeStd [63] |
| fBodyBodyGyroMag mean,std | frequencyBodyBodyGyroscopeMagnitudeMean [64], frequencyBodyBodyGyroscopeMagnitudeStd [65] |
| fBodyBodyGyroJerkMag mean,std | frequencyBodyBodyGyroscopeJerkMagnitudeMean [66], frequencyBodyBodyGyroscopeJerkMagnitudeMean [67] |

Tidy data set contains average of each variable for each `activity [68]` and each `subject [1]`.










