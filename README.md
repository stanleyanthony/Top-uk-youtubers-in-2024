# Analyzing The Top YouTubers In UK 2024


## Project Overview

- The pain point

TheHead of marketing wants to find out who are the top YouTubers in the United Kingdon, as this will help the marketing team make informed decisions on which YouTuber will be best to run marketing campaign and partnerships with throughout the year.

- The ideal solution

To create a dashboard that provide insights into the top YouTubers in the United Kingdom. This dashboard should include:
1. Subscriber count
2. Total views
3. Total videos
4. Views engagement rate

These key metrics will help decide on which YouTuber to collaborate with to run marketing campaigns.


## User Story

As the Head of Marketing, I want to use a dashboard that analyses YouTube channel data in the United Kingdom.
This dashboard should allow me to identify the top performing channels based on metrics like subscriber base and average views.
With this information, I can make more informed decisions about which Youtubers are best to collaborate with, and therefore maximize how effective each marketing campaign is.


## Data Source

We need data of the top 100 YouTubers in the United Kingdom in 2024, that includes:

1. The channel names
2. Number of videos uploaded
3. Total subscribers
4. Total views

This data is sourced from Kaggle [Get it here!](https://www.kaggle.com/datasets/bhavyadhingra00020/top-100-social-media-influencers-2024-countrywise?resource=download)


## Tools

| Tools | Purpose |
| ----- | ------- |
| Excel | Exploring the data and testing |
| Sql Server | Cleaning, testing, and analyzing the data |
| Power BI | Visualing the data through interactive dashboard |
| GitHub | Hosting projects documentation and version control |


## Stages for Analysis

- Design
- Development
- Testing
- Analysis


## Design


### Dashboard Component Requirements

- First we firgured out what the dashboard should contain based on the requirements provided?
To understand what it should contain, we need to figure out what questions we need the dashboard to answer:

1. Who are the top 10 YouTubers with the most subscribers?
2. Which 3 channels have uploaded the most videos?
3. Which 3 channels have the most views?
4. Which 3 channels have the highest average views per video?
5. Which 3 channels have the highest views per subscriber ratio?
6. Which 3 channels have the highest subscriber engagement rate per video uploaded?

For now, these are some of the questions we need to answer, this may change as we progress down our analysis.


## Development


### Pseodocode 

- What's the general approach in creating this solution from start to finish?

1. Get the data
2. Explore the data in Excel
3. Load the data into SQL Server
4. Clean the data with SQL
5. Test the data with SQL
5. Visualize the data in Power BI
6. Generate the findings based on the insights
7. Write the documentation + commentary
8. Publish the data to GitHub Pages


### Data Exploration Note 

This is the stage where you have a scan of what's in the data, errors, inconcsistencies, bugs, weird and corrupted characters etc

- What are your initial observations with this dataset? What's caught your attention so far?

1. There are at least 4 columns that contain the data we need for this analysis, which signals we have everything we need from the file without needing to contact the client for any more data.

2. The first column contains the channel ID with what appears to be channel IDS, which are separated by a @ symbol - we need to extract the channel names from this.

3. Some of the cells and header names are in a different language - we need to confirm if these columns are needed, and if so, we need to address them.

4. We have more data than we need, so some of these columns would need to be removed.


### Data Cleaning 

1. What do we expect the clean data to look like? (What should it contain? What contraints should we apply to it?)
The aim is to refine our dataset to ensure it is structured and ready for analysis.

The cleaned data should meet the following criteria and constraints:

1. Only relevant columns should be retained.
2. All data types should be appropriate for the contents of each column.
3. No column should contain null values, indicating complete data for all records.

Below is a table outlining the constraints on our cleaned dataset:

| Property | Constraint |
| -------- | ---------- |
| Number of rows | 100 |
| Number of column | 4 |

And here is a tabular representation of the expected schema for the clean data:

 What steps are needed to clean and shape the data into the desired format?
1. Remove unnecessary columns by only selecting the ones you need
2. Extract Youtube channel names from the first column
3. Rename columns using aliases




















