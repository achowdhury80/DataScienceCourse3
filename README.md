# Instructions to retrieve tidy dataset
#### Execute run_analysis.R to retrieve clean data set.
#### Currently it uses the URL https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip to retrieve raw data.
#### Please change the url if the source has changed.
#### It creates data directory under R execution working directory. Please change the value of the variable 'dataDirectory' in the script to use different data location.
#### Under data directory, it downloads the source file and unzips it.
#### At the end it creates a file 'tidyData.txt' under data dataDirectory. Please modify the value of the variable 'tidyDataFileName' to use different file name.
#### The script will add two data frames into the execution environment namely 'tidyData', 'merged_data'. 
#### 'tidyData' is a data frame for the tidy dataset.
#### 'merged_data' is a data frame before applying grouping and calculating mean.
