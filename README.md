# Spotify Year-in-Review: Data Science and Visualization of Personal Listening Trends with Python and Tableau
⭐️[Tableau Dashboard](https://public.tableau.com/shared/HHJ3PJZXJ?:display_count=n&:origin=viz_share_link)⭐️

## Introduction: 
This project offers a comprehensive analysis of a Spotify listening history dataset to uncover personal listening trends over the past year. By leveraging Python for data processing and Tableau for visualization, the project provides insights into favorite artists, seasonal listening habits, peak times for music, and much more. Designed for music enthusiasts and data analysts, this notebook aims to uncover hidden patterns in music consumption and showcase these trends in an engaging, interactive format.

## Dataset:
The dataset, sourced from Spotify’s user data access options, contains the following fields:

* Timestamps of each listening session (endTime)
* Artist names and track names for each song
* Listening duration (in milliseconds, seconds, and minutes)
* Date and time details including day, month, and hour for trend analysis
* Seasonal attributes such as the season and day of the week
* The dataset contains over 32,000 entries, which allows for a robust exploration of listening behaviors over time.

## Technologies Used:

* Python
  * pandas: For data manipulation and cleaning
  * numpy: For efficient numerical operations
  * matplotlib & seaborn: For initial data visualizations and analysis
* Tableau: For creating an interactive dashboard to explore trends more dynamically

## Data Collection: 
* Data was downloaded directly from Spotify’s user account portal, which allows users to export their listening history. This data represents a comprehensive log of every track played, including details on the time, artist, and duration.

## Data Preparation: 
Data cleaning and preparation were essential steps to ensure accuracy and relevance for analysis. Using Pandas in Google Colab, the following tasks were performed:

* Data Parsing: Converted timestamps to date formats for day, month, and seasonal analysis.
* Duration Conversion: Converted listening duration from milliseconds to seconds and minutes for more intuitive understanding.
* Datetime Features: Extracted features like dayOfWeek, hour, month, and season_listening for time-based analysis.

## Exploratory Analysis: 
Using Python libraries, initial data exploration provided key insights:

* Top Artists and Tracks: Identified frequently listened-to artists and tracks to get an overview of favorite music.
* Listening Patterns: Analyzed data by the day of the week and hour of the day to find peak listening times.
* Seasonal Trends: Observed changes in listening behavior across different seasons (e.g., Winter, Spring, Summer, Autumn).

## Dataframes Creation: 
To streamline the analysis, various new DataFrames were created to address specific analytical needs:

* Daily Listening Trends: Summarized listening time by day to track day-to-day variation.
* Monthly Trends: Aggregated data by month to study long-term listening patterns.
* Seasonal Listening Trends: Categorized data by season to highlight seasonal preferences and changes.
* Hourly Listening Activity: Created a DataFrame that focused on the hour of the day to identify peak listening hours.

## Visualizations:
* Python Visualizations: Initial data visualization in Google Colab provided a basis for understanding core listening habits.

* [Tableau Dashboard](https://public.tableau.com/shared/HHJ3PJZXJ?:display_count=n&:origin=viz_share_link)

## Notable Findings
Several interesting insights were uncovered through this analysis:

* Seasonal Trends: Certain artists had peaks during specific times of the year. For example, Taylor Swift's music was most frequently played in spring and autumn, while tracks by Drake and Nicki Minaj peaked in autumn and winter respectively. 
* Top Artists and Tracks: The most frequently played artists included Taylor Swift, Drake, Nicki Minaj, Tate McRae, and Sabrina Carpenter.
* Peak Listening Hours: Most listening occurred after 1pm, suggesting music as a common afternoon and evening activity.
* Weekly Patterns: Monday, Tuesday, and Friday saw higher listening volumes, which aligns with typical weekday routines where people might use music to boost focus at the start of the week or unwind as they approach the weekend.

## Future Work:
This project opens the door to several additional analysis avenues:

* Sentiment Analysis: Performing a sentiment analysis on song lyrics to see if seasonal moods correlate with lyrical themes.
* Predictive Modeling: Developing models to predict future listening habits based on past trends.
* Genre Analysis: Expanding the dataset with genre labels to explore genre preferences over time and by season.
* Web Application for User Data Upload: Develop this project into a web application where users can upload their Spotify listening data to generate their own personalized year-in-review reports. This app could visualize key metrics like top artists, peak listening times, and seasonal trends, creating a unique, interactive experience for any user interested in analyzing their music habits.

## How to Use:
* Step 1: Download Your Spotify Data
  * Log into your Spotify account on the web.
  * Go to Settings > Account Privacy.
  * Look for the option Download Account Data.
  * To get a more detailed history, select the Download Extended Streaming History option. This will provide a larger pool of data for analysis, though it may take a few more days to reach your inbox.
  * Once requested, Spotify will email you a download link after processing your data. Download the ZIP file from this link.
  * Extract the ZIP file. Inside, you'll find JSON files labeled as StreamingHistory_music_#.json.
* Step 2: Open the Google Colab Notebook
  * Go to Google Colab.
  * Open the notebook file Spotify_Project.ipynb in this Repo and create a copy of it.
  * Familiarize yourself with the notebook interface if needed; each section of the notebook has cells you can run.
* Step 3: Import Your JSON Files into Google Colab
  * Click on Choose Files and upload all of your StreamingHistory_music_#.json files.
  * Ensure all the JSON files are successfully uploaded; you should see them listed under the Files section on the left sidebar.
* Step 4: Run All Cells in the Notebook
  * Once the JSON files are uploaded, go to the Runtime menu in Colab.
  * Select Run All to execute each cell in sequence.
  * The code will process the JSON data, analyze it, and output visualizations and summaries. These typically include:
   * Top Artists: List of your most-listened-to artists.
   * Top Songs: List of your most-played songs.
   * Listening Hours: Insights into the times of day you listen most.
   * Seasonal Listening Habits: Analysis of how your listening varies across different seasons.
* Step 5: Review and Interpret Your Results
  * Once all cells have run, scroll through the outputs to explore the visualizations and data insights. This analysis will help you see trends and patterns in your Spotify listening habits.
  * A complete CSV of your data will appear in the left-hand sidebar under Files. Although I plan to add more visualizations within the code, you can download this data and use it with any visualization tools of your choice for further analysis. For this project, I used Tableau.
