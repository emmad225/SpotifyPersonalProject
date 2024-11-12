# Spotify Year-in-Review Analysis; Exploring My Personal Music Listening Trends Using Python and Tableau

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

* Python 3.7 or higher: For data loading, cleaning, analysis, and visualization
* Tableau: For creating an interactive dashboard to explore trends more dynamically
* Libraries
** pandas: For data manipulation and cleaning
** numpy: For efficient numerical operations
** matplotlib & seaborn: For initial data visualizations and analysis

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
* Python Visualizations
Initial data visualization in Google Colab provided a basis for understanding core listening habits.

* Tableau Dashboard
An interactive dashboard was developed in Tableau to enhance data exploration.
LINK HERE

## Notable Findings
Several interesting insights were uncovered through this analysis:

* Seasonal Trends: Certain artists had peaks during specific times of the year. For example, Taylor Swift's music was most frequently played in spring autumn, while tracks by Drake and Nicki Minaj had peaks in autumn and winter respectively. 
*Top Artists and Tracks: The most frequently played artists included Taylor Swift, Drake, Nicki Minaj, Tate McRae, and Sabrina Carpenter.
* Peak Listening Hours: Most listening occurred in the afternoon and evenings, particularly after 1pm, suggesting music as a common evening activity.
* Weekly Patterns: Monday, Tuesday, and Friday saw higher listening volumes, which aligns with typical weekday routines where people might use music to boost focus at the start of the week or unwind as they approach the weekend.

Future Work:
This project opens the door to several additional analysis avenues:

* Sentiment Analysis: Performing a sentiment analysis on song lyrics to see if seasonal moods correlate with lyrical themes.
* Predictive Modeling: Developing models to predict future listening habits based on past trends.
* Genre Analysis: Expanding the dataset with genre labels to explore genre preferences over time and by season.

Tableau Dashboard: LINK
