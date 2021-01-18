# Code book for Coursera Getting and Cleaning Data course project
The data set that this code book pertains to is located in the `MeanData.txt` file of this repository.

See the `README.md` file of this repository for background information on this data set.

The structure of the data set is described in the `Data` section, its variables are listed in the `Variables` section, and the transformations that were carried out to obtain the data set based on the source data are presented in the `Transformations` section.

## Data
The `MeanData.txt` data file is a text file, containing space-separated values.

The first row contains the names of the variables, which are listed and described in the `Variables` section, and the following rows contain the values of these variables.

## Variables
Each row contains, for a given subject and activity, 79 averaged signal measurements.

### Identifiers
* `subject`: Subject identifier, integer, ranges from 1 to 30.

* `activity`: Activity identifier, string with 6 possible values:

  * `WALKING`: subject was walking
  * `WALKING_UPSTAIRS`: subject was walking upstairs
  * `WALKING_DOWNSTAIRS`: subject was walking downstairs
  * `SITTING`: subject was sitting
  * `STANDING`: subject was standing
  * `LAYING`: subject was laying
  
### Average of measurements
All measurements are floating-point values, normalised and bounded within [-1,1].

Prior to normalisation, acceleration measurements (variables containing Accelerometer) were made in g's (9.81 m.s⁻²) and gyroscope measurements (variables containing Gyroscope) were made in radians per second (rad.s⁻¹).

Magnitudes of three-dimensional signals (variables containing Magnitude) were calculated using the Euclidean norm.

The measurements are classified in two domains:

* Time-domain signals (variables prefixed by `time`), resulting from the capture of accelerometer and gyroscope raw signals.

* Frequency-domain signals (variables prefixed by `frequency`), resulting from the application of a Fast Fourier Transform (FFT) to some of the time-domain signals.

### Time-domain signals
* Average time-domain body acceleration in the X, Y and Z directions:
  * `timeBodyAccMeanX`
  * `timeBodyAccMeanY`
  * `timeBodyAccMeanZ`
  
* Standard deviation of the time-domain body acceleration in the X, Y and Z directions:
  * `timeBodyAccStdX`
  * `timeBodyAccStdY`
  * `timeBodyAccStdZ`
  
* Average time-domain gravity acceleration in the X, Y and Z directions:
  * `timeGravityAccMeanX`
  * `timeGravityAccMeanY`
  * `timeGravityAccMeanZ`
  
* Standard deviation of the time-domain gravity acceleration in the X, Y and Z directions:
  * `timeGravityAccStdX`
  * `timeGravityAccStdY`
  * `timeGravityAccStdZ`
  
* Average time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
  * `timeBodyAccJerkMeanX`
  * `timeBodyAccJerkMeanY`
  * `timeBodyAccJerkMeanZ`
  
* Standard deviation of the time-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
  * `timeBodyAccJerkStdX`
  * `timeBodyAccJerkStdY`
  * `timeBodyAccJerkStdZ`
  
* Average time-domain body angular velocity in the X, Y and Z directions:
  * `timeBodyGyroMeanX`
  * `timeBodyGyroMeanY`
  * `timeBodyGyroMeanZ`
  
* Standard deviation of the time-domain body angular velocity in the X, Y and Z directions:
  * `timeBodyGyroStdX`
  * `timeBodyGyroStdY`
  * `timeBodyGyroStdZ`
  
* Average time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:
  * `timeBodyGyroJerkMeanX`
  * `timeBodyGyroJerkMeanY`
  * `timeBodyGyroJerkMeanZ`
  
* Standard deviation of the time-domain body angular velocity jerk (derivation of the angular velocity in time) in the X, Y and Z directions:
  * `timeBodyGyroJerkStdX`
  * `timeBodyGyroJerkStdY`
  * `timeBodyGyroJerkStdZ`
  
* Average and standard deviation of the time-domain magnitude of body acceleration:
  * `timeBodyAccMagMean`
  * `timeBodyAccMagStd`
  
* Average and standard deviation of the time-domain magnitude of gravity acceleration:
  * `timeGravityAccMagMean`
  * `timeGravityAccMagStd`
  
* Average and standard deviation of the time-domain magnitude of body acceleration jerk (derivation of the acceleration in time):
  * `timeBodyAccJerkMagMean`
  * `timeBodyAccJerkMagStd`
  
* Average and standard deviation of the time-domain magnitude of body angular velocity:
  * `timeBodyGyroMagMean`
  * `timeBodyGyroMagStd`
  
* Average and standard deviation of the time-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):
  * `timeBodyGyroJerkMagMean`
  * `timeBodyGyroJerkMagStd`
  
### Frequency-domain signals

* Average frequency-domain body acceleration in the X, Y and Z directions:
  * `frequencyBodyAccMeanX`
  * `frequencyBodyAccMeanY`
  * `frequencyBodyAccMeanZ`
  
* Standard deviation of the frequency-domain body acceleration in the X, Y and Z directions:
  * `frequencyBodyAccStdX`
  * `frequencyBodyAccStdY`
  * `frequencyBodyAccStdZ`
  
* Weighted average of the frequency components of the frequency-domain body acceleration in the X, Y and Z directions:
  * `frequencyBodyAccMeanFreqX`
  * `frequencyBodyAccMeanFreqY`
  * `frequencyBodyAccMeanFreqZ`
  
* Average frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
  * `frequencyBodyAccJerkMeanX`
  * `frequencyBodyAccJerkMeanY`
  * `frequencyBodyAccJerkMeanZ`
  
* Standard deviation of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
  * `frequencyBodyAccJerkStdX`
  * `frequencyBodyAccJerkStdY`
  * `frequencyBodyAccJerkStdZ`
  
* Weighted average of the frequency components of the frequency-domain body acceleration jerk (derivation of the acceleration in time) in the X, Y and Z directions:
  * `frequencyBodyAccJerkMeanFreqX`
  * `frequencyBodyAccJerkMeanFreqY`
  * `frequencyBodyAccJerkMeanFreqZ`
  
* Average frequency-domain body angular velocity in the X, Y and Z directions:
  * `frequencyBodyGyroMeanX`
  * `frequencyBodyGyroMeanY`
  * `frequencyBodyGyroMeanZ`
  
* Standard deviation of the frequency-domain body angular velocity in the X, Y and Z directions:
  * `frequencyBodyGyroStdX`
  * `frequencyBodyGyroStdY`
  * `frequencyBodyGyroStdZ`
  
* Weighted average of the frequency components of the frequency-domain body angular velocity in the X, Y and Z directions:
  * `frequencyBodyGyroMeanFreqX`
  * `frequencyBodyGyroMeanFreqY`
  * `frequencyBodyGyroMeanFreqZ`
  
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration:
  * `frequencyBodyAccMagMean`
  * `frequencyBodyAccMagStd`
  * `frequencyBodyAccMagMeanFreq`
  
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body acceleration jerk (derivation of the acceleration in time):
  * `frequencyBodyAcceJerkMagMean`
  * `frequencyBodyAcceJerkMagStd`
  * `frequencyBodyAcceJerkMagMeanFreq`
  
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity:
  * `frequencyBodyGyroMagMean`
  * `frequencyBodyGyroMagStd`
  * `frequencyBodyGyroMagMeanFreq`
  
* Average, standard deviation, and weighted average of the frequency components of the frequency-domain magnitude of body angular velocity jerk (derivation of the angular velocity in time):
  * `frequencyBodyGyroJerkMagMean`
  * `frequencyBodyGyroJerkMagStd`
  * `frequencyBodyGyroJerkMagMeanFreq`
  
## Transformations
The zip file containing the source data is located at https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.

The following transformations were applied to the source data:
1. Merges the `training` and the `test` sets to create one data set.

2. The measurements on the `mean` and `standard` deviation (i.e. signals containing the strings `mean` and `std`) were extracted for each measurement, and the others were discarded.

3. The activity identifiers (originally coded as integers between 1 and 6) were replaced with descriptive activity names (see Identifiers section).

4. The variable names were replaced with descriptive variable names (e.g. `tBodyAcc-mean()-X` was modified to `timeBodyAccMeanX`), using the following set of rules:
  * Special characters (i.e. `()`, and `-`) were removed
  * `mean` and `std` were replaced with `Mean` and `Std` respectively
  * `t` and `f` were replaced with `time` and `frequency`
  
5. From the data set in step 4, the final data set was created with the average of each variable for each activity and each subject.

The collection of the source data and the transformations listed above were implemented by the `run_analysis.R` script (see `README.md` file for usage instructions).
