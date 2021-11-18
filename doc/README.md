# CPSC292Project2

This project was about applying the skills we have learned in Unit 3 in order to make our project 1 easier to understand, return to, and 	read. We did this by refactoring, as well as making changes to the code using loops and functions. Overall, the code went from 941 to 152 lines!

We made a few substantial changes to our code in order to help clean it up and condense it. Initially, we realized that there were a lot of instances for our first visual where we needed to copy and paste the same code 27 times, changing one number, on multiple occasions. So, we added a for-loop that does the following for each year of the data set: It creates an intermediate data frame for each year, it isolates the specific year to clean the data, renumbers the rows, sums the columns, and combines the data with a dataframe of the different countries into one data frame called “malaria.all.X” (X = year). This essentially saved us many lines of code that we needed in order to clean up the data set for use in the creation of our graph. More importantly, this helped optimize ram as the number of dataframes required were cut in half. The lines of code for this for-loop range from lines 85 to 92. 

Next, we created a function, “Malria.Map.F,” that made it easier to save each map’s .png. The function took three inputs, the dataframe being converted into a map, the year for which the map corresponded to, and the name of the file the user wishes to save each individual map as. By creating this function, we were able to consolidate the code by only needing to modify the year in three different places. Previously, each map’s code was 14 lines (27 x 14 = 378 lines of code to make all maps). By using this function, each map could be made with the use of one line. The function can be found from lines 32 to 56 with detailed notes of what each line represents. 

Although the function helped alleviate the tedious edits we had to do for each map, we still found ourselves copying and pasting the function 27 different times.This influenced our third change, which was creating a for-loop that runs the function mentioned above for each year in the data set. This made the function automatically run for each year, while still consolidating the code further. The lines for this for-loop range from lines 98 to 104. 

Please note that all results for visual 1 can be found in the folder “results.” The graph created for visual 2 is presented on the RMD file when the code is run. 

If any questions, concerns, or bugs arise, please feel free to reach out to us:

Mo Hijazi - mhijazi@chapman.edu

Todd Soo- tsoo@chapman.edu

