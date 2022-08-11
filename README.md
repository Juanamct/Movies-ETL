# Movies-ETL

## Overview: Create an automated pipeline that takes in new data, performs the appropriate transformations, 
## and loads the data into existing tables
  1. Write an ETL Function to Read Three Data Files 
  2. Extract and Transform the Wikipedia Data
  3. Extract and Transform the Kaggle data
  4. Create the Movie Database

 ###Method: Using Python, Pandas, the ETL process, and code refactoring

  ### Data 1: Write an ETL Function to Read Three Data Files: write a function that reads in the three data 
  ###         files and creates three separate DataFrames.
    		        - set the three variables for the files equal to the function that read in the three files and 
                  gave it a name. 
                - reassign the variable names to allow you to display each DataFrame.    		
    
  ### Data 2: Extract and Transform the Wikipedia Data:
    		        - extract and transform the Wikipedia data so you can merge it with the Kaggle metadata,
                  while extracting the IMDb IDs using a regular expression string and dropping duplicates.
                - use a try-except block to catch errors.
                - Convert the cleaned Wikipedia data to a Pandas DataFrame, and the DataFrame is displayed
 
  ### Data 3: Extract and Transform the Kaggle data: 
    		        - extract and transform the Kaggle metadata and MovieLens rating data, 
                - convert the transformed data into separate DataFrames
                - merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df 
                  DataFrame.
                - merge the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df

  ### Data 4: Create the Movie Database:
                - add the movies_df DataFrame and MovieLens rating CSV data to a SQL database
    		        - replace the current data in the movies table in the SQL database with data from the movies_df DataFrame 
                - add data from the MovieLens rating CSV file to the ratings table in the SQL database
