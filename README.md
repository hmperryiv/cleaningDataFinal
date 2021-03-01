# cleaningDataFinal

#  This is one script to execute the whole thing.

#  The output will be in the '/results' folder, if there is a problem the
#  results folder has also been uploaded to GITHUB.

#  When completed it will produce a folder called 'results', this folder will 
#  contain the following:
#     test(or train)_combinded_data_set.csv: this is the combined data sets for 
#                                            either group only.
#     combined_data_set.csv: This is both test and train complete data sets
#                            merged into one csv (meets objective 1, 3, 4)
#     combined_mean_std_dev_data_set: both test and train group, but only
#                                     elements from their data sets that were
#                                     either means or std dev 
#                                     (meets objective 2,3,4)
#     avg_measurements_by_subject_and_activity_data_set.csv: average of each 
#                                     variable for each activity and each subject.
#                                     (meets objective 3,4,5)


# **** REQUIRED LIBRARIES ****
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