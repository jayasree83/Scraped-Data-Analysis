# Scraped-Data-Analysis from Youtube for colleges in Missouri, Kansas Area
This project involves gathering and analyzing YouTube data for multiple colleges in the Kansas and Missouri area using the YouTube Data API v3. The data collected includes information about the colleges' YouTube channels, such as subscribers, views, and total videos, as well as detailed insights about the videos uploaded by these channels.

# Overview
This project uses the YouTube Data API to:
  Retrieve basic statistics for the YouTube channels of several colleges in the Kansas and Missouri area.
  Extract detailed statistics about individual videos, such as views, likes, and comments.
  Analyze video publication trends over time.
  Visualize the data using bar plots to compare different channels and videos.
The goal is to compare the YouTube presence of multiple colleges and provide insights based on the data.

# Colleges Analyzed
The following colleges were selected for the analysis:
  University of Central Missouri (UCMO)
  University of Missouri-Kansas City (UMKC)
  Rockhurst University
  University of Missouri (UOM)
  Webster University
  Saint Louis University

# Pre-requisites
**Python**: This project uses Python, so make sure you have Python installed on your system.
**Google API Key**: You will need a Google API key to access the YouTube Data API v3..
**Required Libraries**: google-api-python-client, pandas, seaborn, matplotlib (optional for custom plots)

# SetUp
1. Obtaining YouTube Data API key: In the Google Cloud Console, go to APIs & Services > Search for YouTube Data API v3.
   Create credentials and generate the custom API Key. This will be used to authenticate your API requests.
2. Run the script: The script is designed to be run in a Python environment.
3. Output: The script will generate a CSV file. My script was specific to UCMO- Video_Details(UCMO).csv

# Funtions
1. get_channel_stats(youtube, channel_ids): 
   This function retrieves basic statistics about the specified YouTube channels, including:
      Channel Name
      Subscriber Count
      Total Views
      Total Videos
2. get_video_ids(youtube, playlist_id): This function fetches the list of video IDs from the playlist associated with each channel.
3. get_video_details(youtube, video_ids):
   This function retrieves detailed information about the videos, including:
      Video Title
      Published Date
      View Count
      Like Count
      Comment Count
4. Data Visualisations
   The following visualizations are generated:
      Bar plots comparing the subscriber counts, views, and total videos across different channels.
      Top 10 videos sorted by the number of views.
      Monthly video publication trend, showing how many videos were published each month.
