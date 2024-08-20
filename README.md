# data-sourcing-challenge
We have been tasked to prepare some data for a recommendation system to help people find movie reviews and related movies. We extracted data from two different sources: The New York Times API and The Movie Database, then we merged the data together. The text extracted from these APIs was later used with natural language processing methods.
What did we do?
This Challenge had three parts, that had to be completed in order:

Part 1: Access the New York Times API.
Create an empty list called reviews_list to store the reviews you retrieve from the API.
Previewed the first five results in JSON format using json.dumps with the argument indent=4 to format the data.

Convert reviews_list to a Pandas DataFrame using json_normalize()

Extract the movie title from the "headline.main" column and save it to a new column "title". To do this, you will use the Pandas apply() method and the following lambda function:

Part 2: Access The Movie Database API.
Create an empty list called tmdb_movies_list to store the results from your API requests. This will contain a list of dictionaries.

Create a variable called request_counter and initialize it with the value of 1.

Part 3: Merge and Clean the Data for Export.
Loop through the titles list created from the movie reviews DataFrame, and perform the following actions:

Perform the actions outlined in Step 2.

Perform a GET request that sends the title to The Movie Database search and retrieves the JSON results.
Merge the New York Times reviews and TMDB DataFrames on the title column.

The genres, spoken_languages, and production_countries columns were saved as lists, but we want the columns to be strings without the list characters ([, ], and ').