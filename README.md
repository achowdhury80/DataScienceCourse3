## Instructions to retrieve tidy dataset

* Execute 'run_analysis.R' to retrieve tidy data set. 
* To execute the script, put 'run_analysis.R' in R working directory and run the command - "source('run_analysis.R');".
* Currently it expects source file as an archive file with name 'UCIData.zip'.
* Please modify the value of variable 'sourceZipFileName' in the script if the source file name is different.
* It unzips the archive file.
* The script will add a data frame into the execution environment namely 'tidyData'. 
* 'tidyData' is a data frame for the tidy dataset.
* At end, it recursively deletes the unzipped folder.

