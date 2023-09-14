# Youtube-data-harvesting
YouTube Data Harvesting and Warehousing
Overview
This project is designed to collect data from YouTube channels, store it in a MongoDB database, and perform various analyses on the collected data. It uses Python and several libraries and APIs, including the Google YouTube API, pymongo, psycopg2, pandas, and Streamlit.

Table of Contents
Prerequisites
Installation
Usage
Functionality
Database Schema
Analysis Queries
Contributing
License
Prerequisites
Before using this code, ensure you have the following dependencies installed:

Python 3.x
MongoDB
PostgreSQL
Required Python libraries (specified in the code)
Installation
Clone this repository to your local machine.
git clone <repository_url>
Install the required Python libraries.

pip install pymongo psycopg2 pandas streamlit google-api-python-client isodate pillow certifi

Set up your MongoDB and PostgreSQL databases.

Obtain a Google API key for the YouTube Data API and replace api_key in the code with your API key.

Configure your database connection parameters in the code (host, user, password, port, database).

Usage
Run the Python script to collect data from YouTube channels and store it in the MongoDB database.
python your_script_name.py
Launch the Streamlit web application to interact with the collected data and perform analyses.
streamlit run your_streamlit_app.py

Functionality
Collects channel details, playlists, videos, and comments from YouTube.
Stores the collected data in MongoDB and PostgreSQL databases.
Provides a Streamlit-based web interface for querying and analyzing the data.
Offers various predefined analysis queries to gain insights into the YouTube data.
Database Schema
The code creates the following tables in PostgreSQL:

channels: Stores channel details.
playlists: Stores playlist details.
videos: Stores video details.
comments: Stores video comments.
Analysis Queries
The Streamlit web application offers the following predefined analysis queries:

List all video titles and their corresponding channel names.
Identify channels with the most number of videos and their counts.
Find the top 10 most viewed videos and their respective channels.
Count the number of comments on each video and display the video names.
Discover videos with the highest number of likes and their corresponding channel names.
Calculate the total number of likes for each video and display the video names.
Determine the total number of views for each channel and display the channel names.
List channels that published videos in the year 2022.
Calculate the average duration of videos in each channel.
Contributing
Contributions to this project are welcome. If you find any issues or want to enhance its functionality, please create a pull request or open an issue.
