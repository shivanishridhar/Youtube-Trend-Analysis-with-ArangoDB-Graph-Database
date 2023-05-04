# Youtube-Trend-Analysis-with-ArangoDB-Graph-Database
## Problem Statement
Youtube is the most widely used and popular streaming platform in the world today. For a video to 
reach to maximum people, YouTube offers a trending page on website that shows videos which are 
trending at that particular time. Other than few viral videos that achieve high traction which are 
predictable to end up in trending section, rest of the videos cannot be predicted. In some cases, the 
videos achieve traction at a later stage and this analysis is usually difficult to track. Hence , a multimodel 
database that deals with analysis of YouTube Data on Trending Videos is introduced in this project.

## Data Architecture

![Data Architecture](https://user-images.githubusercontent.com/114179722/236095375-90d3f4bc-7743-48a3-9f2f-d9ec677d7a75.jpg)

Data Source –Data source primary will be consisting of Kaggle datasets and JSON file which has been scraped from the YouTube API.
Potential Kaggle dataset - https://www.kaggle.com/datasets/rsrishav/youtube-trending-videodataset?select=CA_youtube_trending_data.csv

Data Ingestion – Data processing will be done by a python script which will combine data from Kaggle and YouTube API. 
The preprocessed data will be integrated with Arango DB with the help of ETL tool (Talend). This will help to ingest preprocessed JSON file into Arango DB.

Data Storage and Querying – Arango DB will help to store the data in the form of JSON which will be used for further analysis which is YouTube Trends for videos. The data Analysis will take place with the help of queries as well with the Machine Learning algorithms.

Data Reporting –
Visualizations of the preprocessed data will be created by Power BI with the help of different graphs. The Visualizations will be pushed to Users to make them understand the YouTube trends in graphical representations.

Users –
Users will be able to give queries in the Arango DB to extract information as per their requirements. 
Users will also be able to see the visualizations created by Power BI

