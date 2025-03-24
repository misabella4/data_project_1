# Data Project 1

Original project proposal:
I am going to see if there is a correlation between the most popular artists of 2024 on a streaming app like Spotify vs how often they appear on the Billboard top 100 chart. I will use this API: https://developer.spotify.com/documentation/web-api/tutorials/getting-started to find an artist's popularity and see if the most popular artists appear more often on the chart. I will use a CSV file with the Billboard top 100 songs and pull the artists off that as data to compare. I can create the CSV manually in Excel using the chart I find online. As for the Spotify API, it's open source if you have an account, but I'll use cURL to make the API calls. All instructions can be found in the link above.

# Step 1: Setting Up Environment
- Created new repo 'data_project_1' on GitHub
- Set up notebook in Google Colab and installed necessary libraries
- Create free Spotify account to get access key for API data

# Step 2: Getting Billboard Top 100 Data
- Manually created a CSV file on Google Sheets with https://www.billboard.com/charts/hot-100/
- Imported CSV into Google Colab to start working with my own data
- Wrote Python code for project setup to make sure all columns and data was working

# Step 3: Data Ingestion
- Used my own CSV file (Billboard chart via Sheets) as one form of data
- Used the Spotify API data as my external source of data
- Brainstormed ways to combine and transform the two datasets as one

# Step 4: Data Transformation
- Get the popularity score for each artist via the data sets
- Give the highest popularity score to songs depending on its rank on both data sets
- Merge the API with Billboard df (from Sheets) to create new column called Popularity Score

# To DO:
- Data Storage section - putting merged data into a SQL database
- Data Summarization section - generating a summary of the ingested and transformed data
- File Format Conversion section - allowing the user to choose the output type they want through Python functions that convert the billboard_df into different formats
- Reflection!!
