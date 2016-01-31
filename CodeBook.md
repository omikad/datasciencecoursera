# Human Activity Recognition Using Smartphones Dataset

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

For full desciption of data open this link:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

# Features

Script `run_analysis.R` will produce file `UCI_HAR_tidy.txt` that contains the following features:

```
[1] "subject"                           
[2] "activity"            
[3] "timeBodyAccelerometerMeanX"                     
[4] "timeBodyAccelerometerMeanY"                     
[5] "timeBodyAccelerometerMeanZ"                     
[6] "timeBodyAccelerometerStdX"                      
[7] "timeBodyAccelerometerStdY"                      
[8] "timeBodyAccelerometerStdZ"                      
[9] "timeGravityAccelerometerMeanX"                  
[10] "timeGravityAccelerometerMeanY"                  
[11] "timeGravityAccelerometerMeanZ"                 
[12] "timeGravityAccelerometerStdX"                   
[13] "timeGravityAccelerometerStdY"                   
[14] "timeGravityAccelerometerStdZ"                   
[15] "timeBodyAccelerometerJerkMeanX"                 
[16] "timeBodyAccelerometerJerkMeanY"                 
[17] "timeBodyAccelerometerJerkMeanZ"                 
[18] "timeBodyAccelerometerJerkStdX"                  
[19] "timeBodyAccelerometerJerkStdY"                  
[20] "timeBodyAccelerometerJerkStdZ"                  
[21] "timeBodyGyroscopeMeanX"                         
[22] "timeBodyGyroscopeMeanY"                         
[23] "timeBodyGyroscopeMeanZ"                         
[24] "timeBodyGyroscopeStdX"                          
[25] "timeBodyGyroscopeStdY"                          
[26] "timeBodyGyroscopeStdZ"                          
[27] "timeBodyGyroscopeJerkMeanX"                     
[28] "timeBodyGyroscopeJerkMeanY"                     
[29] "timeBodyGyroscopeJerkMeanZ"                     
[30] "timeBodyGyroscopeJerkStdX"                      
[31] "timeBodyGyroscopeJerkStdY"                      
[32] "timeBodyGyroscopeJerkStdZ"                      
[33] "timeBodyAccelerometerMagnitudeMean"             
[34] "timeBodyAccelerometerMagnitudeStd"              
[35] "timeGravityAccelerometerMagnitudeMean"          
[36] "timeGravityAccelerometerMagnitudeStd"           
[37] "timeBodyAccelerometerJerkMagnitudeMean"         
[38] "timeBodyAccelerometerJerkMagnitudeStd"          
[39] "timeBodyGyroscopeMagnitudeMean"                 
[40] "timeBodyGyroscopeMagnitudeStd"                  
[41] "timeBodyGyroscopeJerkMagnitudeMean"             
[42] "timeBodyGyroscopeJerkMagnitudeStd"              
[43] "frequencyBodyAccelerometerMeanX"                
[44] "frequencyBodyAccelerometerMeanY"                
[45] "frequencyBodyAccelerometerMeanZ"                
[46] "frequencyBodyAccelerometerStdX"                 
[47] "frequencyBodyAccelerometerStdY"                 
[48] "frequencyBodyAccelerometerStdZ"                 
[49] "frequencyBodyAccelerometerJerkMeanX"            
[50] "frequencyBodyAccelerometerJerkMeanY"            
[51] "frequencyBodyAccelerometerJerkMeanZ"            
[52] "frequencyBodyAccelerometerJerkStdX"             
[53] "frequencyBodyAccelerometerJerkStdY"             
[54] "frequencyBodyAccelerometerJerkStdZ"             
[55] "frequencyBodyGyroscopeMeanX"                    
[56] "frequencyBodyGyroscopeMeanY"                    
[57] "frequencyBodyGyroscopeMeanZ"                    
[58] "frequencyBodyGyroscopeStdX"                     
[59] "frequencyBodyGyroscopeStdY"                     
[60] "frequencyBodyGyroscopeStdZ"                     
[61] "frequencyBodyAccelerometerMagnitudeMean"        
[62] "frequencyBodyAccelerometerMagnitudeStd"         
[63] "frequencyBodyBodyAccelerometerJerkMagnitudeMean"
[64] "frequencyBodyBodyAccelerometerJerkMagnitudeStd" 
[65] "frequencyBodyBodyGyroscopeMagnitudeMean"        
[66] "frequencyBodyBodyGyroscopeMagnitudeStd"         
[67] "frequencyBodyBodyGyroscopeJerkMagnitudeMean"    
[68] "frequencyBodyBodyGyroscopeJerkMagnitudeStd"    
```      

`subject [1]` - integer identifier of person who performed the activity for each window sample. Its range is from 1 to 30. 

`activity [2]` - activity performed by subject: `WALKING`, `WALKING_UPSTAIRS`, `WALKING_DOWNSTAIRS`, `SITTING`, `STANDING`, `LAYING`

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

Original features were renamed to a new set of features:

|Original features|Transformed features|
|-----------------|--------------------|
| tBodyAcc mean,std XYZ | timeBodyAccelerometerMean XYZ [3,4,5], timeBodyAccelerometerStd XYZ [6,7,8] |
| tGravityAcc mean,std XYZ | timeGravityAccelerometerMean XYZ [9,10,11], timeGravityAccelerometerStd XYZ [12,13,14] |
| tBodyAccJerk mean,std XYZ | timeBodyAccelerometerJerkMean XYZ [15,16,17], timeBodyAccelerometerJerkStd XYZ [18,19,20] |
| tBodyGyro mean,std XYZ | timeBodyGyroscopeMean XYZ [21,22,23], timeBodyGyroscopeStd XYZ [24,25,26] |
| tBodyGyroJerk mean,std XYZ | timeBodyGyroscopeJerkMean XYZ [27,28,29], timeBodyGyroscopeJerkStd XYZ [30,31,32] |
| tBodyAccMag mean,std | timeBodyAccelerometerMagnitudeMean [33], timeBodyAccelerometerMagnitudeStd [34] |
| tGravityAccMag mean,std | timeGravityAccelerometerMagnitudeMean [35], timeGravityAccelerometerMagnitudeStd [36] |
| tBodyAccJerkMag mean,std | timeBodyAccelerometerJerkMagnitudeMean [37], timeBodyAccelerometerJerkMagnitudeStd [38] |
| tBodyGyroMag mean,std | timeBodyGyroscopeMagnitudeMean [39], timeBodyGyroscopeMagnitudeStd [40] |
| tBodyGyroJerkMag mean,std | timeBodyGyroscopeJerkMagnitudeMean [41], timeBodyGyroscopeJerkMagnitudeStd [42] |
| fBodyAcc mean,std XYZ | frequencyBodyAccelerometerMean XYZ [43,44,45], frequencyBodyAccelerometerStd XYZ [46,47,48] |
| fBodyAccJerk mean,std XYZ | frequencyBodyAccelerometerJerkMean XYZ [49,50,51], frequencyBodyAccelerometerJerkStd XYZ [52,53,54] |
| fBodyGyro mean,std XYZ | frequencyBodyGyroscopeMean XYZ [55,56,57], frequencyBodyGyroscopeStd [58,59,60] |
| fBodyAccMag mean,std | frequencyBodyAccelerometerMagnitudeMean [61], frequencyBodyAccelerometerMagnitudeStd [62] |
| fBodyBodyAccJerkMag mean,std | frequencyBodyBodyAccelerometerJerkMagnitudeMean [63], frequencyBodyBodyAccelerometerJerkMagnitudeStd [64] |
| fBodyBodyGyroMag mean,std | frequencyBodyBodyGyroscopeMagnitudeMean [65], frequencyBodyBodyGyroscopeMagnitudeStd [66] |
| fBodyBodyGyroJerkMag mean,std | frequencyBodyBodyGyroscopeJerkMagnitudeMean [67], frequencyBodyBodyGyroscopeJerkMagnitudeStd [68] |

Result is tidy data set contains average of each variable for each `activity [2]` and each `subject [1]`.










