This code collects the samsung galaxy data download from coursera. runanalysis.R program will tidy the data set and create a new txt file

Download UCI HAR Dataset zip file and unzip in your local folder, change the setwd to this  UCI HAR Dataset unzipped folder

run runanalysis.R file to find a tidydata.txt file that merged test and train files, aggregated only the mean and standard deviation columns

# lines 10-18

First step is reading all the csv files through read.table

# lines 25-28

Second column bind and row bind the test and train data

# lines 32-39

Third step is labelling the column names using colnames function

# lines 40-44

Fourth step is to replace all the activity column into a meaningful name using gsub function

# lines 47, 48

next step is to grep all the column names that has the word "mean" or "std" in it

# dataset tidydata will have the clean data summarized by mean, std columns

Last step is to aggregate only the columns with mean, and std words and write into a tidydata table
using write.table function



