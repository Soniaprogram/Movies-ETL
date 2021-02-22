# Movies-ETL

## Purpose

to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data and performs the ETL process by adding the data to a PostgreSQL database.

## Analysis

### Deliverable 1: Write an ETL Function to Read Three Data Files
I wrote a function that reads in the three data files and creates three separate DataFrames.
All three DataFrames (wiki_movies_df, Kaggle_metadata, Ratings) are displayed in the ETL_function_test.ipynb file.

### Deliverable 2: Extract and Transform the Wikipedia Data
Using my knowledge of Python, Pandas, the ETL process, and code refactoring, I extracted and transformed the Wikipedia data to merge it with the Kaggle metadata.
The cleaned Wikipedia data is converted to a Pandas DataFrame, and the DataFrame is displayed in the ETL_clean_wiki_movies.ipynb file.

### Deliverable 3: Extract and Transform the Kaggle data
Using my knowledge of Python, Pandas, the ETL process, and code refactoring, I extracted and transformed the Kaggle metadata and MovieLens rating data, then converted the transformed data into separate DataFrames. I merged the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, I merged the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df.
The movies_with_ratings_df and the movies_df DataFrames are displayed in the ETL_clean_kaggle_data.ipynb file.

### Deliverable 4: Create the Movie Database
Use my knowledge of Python, Pandas, the ETL process, code refactoring, and PostgreSQL, I added the movies_df DataFrame and MovieLens rating CSV data to a SQL database.
The data from the movies_df DataFrame replaces the current data in the movies table in the SQL database as displayed in the movies_query.png in the Resources folder.
The data from the MovieLens rating CSV file is added to the ratings table in the SQL database as displayed by the ratings_query.png in the Resources folder.
The elapsed time to add the data to the database is displayed in the ETL_create_database.ipynb file.
