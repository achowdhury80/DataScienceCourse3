## Instructions to retrieve tidy dataset

* Execute 'run_analysis.R' to retrieve tidy data set. 
* To execute the script, put 'run_analysis.R' in R working directory and run the command - "source('run_analysis.R');".
* Currently it expects source file as an archive file with name 'UCIData.zip'.
* Please modify the value of variable 'sourceZipFileName' in the script if the source file name is different.
* It unzips the archive file.
* The script will add a data frame into the execution environment namely 'tidyData'. 
* 'tidyData' is a data frame for the tidy dataset.
* At end, it recursively deletes the unzipped folder.




#### Data clean up steps
Here is the summary of steps.

1. Retrieve the source data in archived from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip.
2. Put the archive file in R working directory.
3. Unzip the file.
4. Load the Test measurements, subjects and activity data from the test directory.
5. Merge the data using column bind. Here we have row by row match for the above three datasets.
6. Load the Train measurements, subjects and activity data from the train directory.
7. Merge the data using column bind. Here we have row by row match for the above three datasets.
8. Combine the test and train datesets using row bind.
9. Load fetures data.
9. Filter the rows which has 'mean' or 'std' in the name.
10. From the combined data set keep the subject, activity and only the features those are selected in the previous step.
11. Load Activity level data.
12. In the combined dataset replace the activity id by activity level.
13.  Appropriately labels the data set with descriptive variable names. 
14.  Group the data based on activity and subject.
15.  Find the mean of all measurement variables. 



