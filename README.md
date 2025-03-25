# Data Project 1

# Original Proposal (via HW check-in):
"I am going to see if there is a correlation between the most popular artists of 2024 on a streaming app like Spotify vs how often they appear on the Billboard top 100 chart. I will use this API: https://developer.spotify.com/documentation/web-api/tutorials/getting-started to find an artist's popularity and see if the most popular artists appear more often on the chart. I will use a CSV file with the Billboard top 100 songs and pull the artists off that as data to compare. I can create the CSV manually in Excel using the chart I find online. As for the Spotify API, it's open source if you have an account, but I'll use cURL to make the API calls. All instructions can be found in the link above."

# Overview
This project finds the correlation between an artist's popularity on Spotify with their frequency of appearance on the Billboard Top 100 chat. I used the Spotify Web API to access data about specific artists found in the Billboard data, and worked to find the most popular artists overall.

# Step 1: Setting Up Environment
- Created new GitHub repo titled 'data_project_1'
- Set up Google Colab notebook with necessary libraries for Python code
- Created a free Spotify Developer account to get API credentials

# Step 2: Getting Billboard Top 100 Data
- Manually created a CSV file on Google Sheets using data from https://www.billboard.com/charts/hot-100/
- Imported CSV into Google Colab
- Wrote Python code to format the columns and values taken in from the file

# Step 3: Data Ingestion
- Loaded the Billboard CSV file into a Pandas df
- Got artists' popularity data using the Spotify API
- Stored popularity in a dictionary to be used later

# Step 4: Data Transformation
- Extracted artists from the Billboard data
- Queried the API to retrieve artist popularities and created a popularity_score variable based on the max artist popularity and rank factor via the Billboard chart
- Merged both data sets into a new df (final_df)
- Sorted songs based on the popularity score

# Step 5: Data Storage
- Used sqlite in Python to turn df into a SQL database
- Created table called Songs with same column names as df

# Step 6: Data Summarization
- Created two new Python functions to summarize and print both dfs
- Cleaned up code and combined everything in one section on Colab notebook
- Correctly found number of number of records and columns for both the ingested and transformed data

# To Do:
- File Format Conversion section - allowing the user to choose the output type they want through Python functions that convert the billboard_df into different formats
- Reflection!!
