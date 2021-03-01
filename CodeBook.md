Steps in execution of script

#Step 0: add libraries

The following librarys are required to run the project, if you don't have them installed below is the commands to install the librarys:

- required libraries
    dplyr
    tibble
    readr
    stringr
    
- R command to install the packages (this is left out of the run_analysis.Rmd file because it adds time to the execution when these are common packages and most should have them):
  install.packages("dplyr")
  install.packages("tibble")
  install.packages("readr")
  install.packages("stringr")
  
#Step 1: Check that the working directory exists, and if it doesn't create it.
#        Switch working directory to the ./data directory

#Step 2: Pull the zip file down from the internet.
#        Unpack the file into the working directory.
#        We will check to see if the file exists, this will accelerate
#        run time after the first run.

#Step 3: Bring all the test participant files into data frames
#        Measurements will be the first read because it's needed by 
#        both test and train participants
#        This will also be morphed into our column names for our X_test (train).txt files
#        Activity Labels will also be done since it is used by both test and train data 
#        sets.

#Step 4: Bring all the train participant files into data frames

#Step 5: Inner Join on Test/Train Activity Number and activity label will merge the 2
#        tables to give descriptions for the activity number, in accordance with item 3
#        of the assignment.

#Step 6: Combine the test data frames, and train data frames into 
#        2 independent data frames

#Step 7: Combine the 2 independent data frames into one data frame, 
#        item 1 of the assignment

#Step 8: clean up the column names

#Step 9: prepare a subset that presents only the means and standard deviations of each
#        activity in accordance with item 2 in the assignment

#Step10: mutate the combinded data set to meet the objectives of item 5 of the assigment.  
#        First, group by subjectnumber, activitynumber, and activitydesc
#        Second, summarise_all columns suing the mean function.

#Step 11: Export the results to the ./result folder