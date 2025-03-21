# Data Project 1

Original project proposal:
I am going to see if there is a correlation between the most popular artists of 2024 on a streaming app like Spotify vs how often they appear on the Billboard top 100 chart. I will use this API: https://developer.spotify.com/documentation/web-api/tutorials/getting-started to find an artist's popularity and see if the most popular artists appear more often on the chart. I will use a CSV file with the Billboard top 100 songs and pull the artists off that as data to compare. I can create the CSV manually in Excel using the chart I find online. As for the Spotify API, it's open source if you have an account, but I'll use cURL to make the API calls. All instructions can be found in the link above.

# Step 1: Setting Up Environment
- Created repo on GitHub
- Set up notebook in Google Colab and installed necessary libraries
- Create Spotify account and get API key for Spotify data

# Step 2: Getting Billboard Top 100 Data
- Manually created a CSV file on Google Sheets with https://www.billboard.com/charts/hot-100/
- Import CSV into Google Colab to start getting data
- Work on Python code for project setup

# Step 3: Data Ingestion
- Local CSV file (Billboard chart from Excel)
- External source (Spotify API)

# Step 4: Data Transformation
- Get popularity score for each artist
- Give highest popularity score to each song
- Merge API with Billboard df and create new popularity score column
