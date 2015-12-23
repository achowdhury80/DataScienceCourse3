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
Here is the summary of steps executed in the script.

1. Unzip the file.
2. Load the Test measurements, subjects and activity data from the test directory.
3. Merge the data using column bind. Here we have row by row match for the above three datasets.
4. Load the Train measurements, subjects and activity data from the train directory.
5. Merge the data using column bind. Here we have row by row match for the above three datasets.
6. Combine the test and train datesets using row bind.
7. Load fetures data.
8. Filter the rows which has 'mean' or 'std' in the name.
9. From the combined data set keep the subject, activity and only the features those are selected in the previous step.
10. Load Activity level data.
11. In the combined dataset replace the activity id by activity level.
12.  Appropriately labels the data set with descriptive variable names. 
13.  Group the data based on activity and subject.
14.  Find the mean of all measurement variables. 



