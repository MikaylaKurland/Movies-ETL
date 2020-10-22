# Movies-ETL

This project is to practice the "Extract, Transform, Load" on three sets of data. The first is a webscrape of movie data from Wikipedia in the form of a JSON, the second is a movie meta_data set and ratings information that I was able to download from Kaggle. The purpose was not to analyze the data, but to create a clean data set that could be worked with.

The process started with looking at and analysing the useful information and determining how it was best to merge it, eventually settling on IMDB identifiers as unique values to determine each film. Then we went about parsing and analysing the data in each set to make sure it was clean and there weren't any errors in pulling it through. 
Examples of this are: Deleting all entries with an episode count, determining and eliminating alternate titles for the same film, making sure columns had squivilent formatting, etc. 

Once this was complete, I merged the data set and uploaded it to PGAdmin, where any analysis could take place.

The original broken down process of cleaning the data is in my "Module Work" ipynb file. The code was refactored into a function to read the three data sets and upload the finished product to PGAdmin, and this final version can be found in "ETL_create_database."
