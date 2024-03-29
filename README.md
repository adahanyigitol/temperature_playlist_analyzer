# temperature_playlist_analyzer
A Spotify Playlist Analyzer for Weather Condition

# Spotify Weather-Based Music Recommender

## Overview

This Python program, dubbed **Spotify Weather-Based Music Recommender**, is the go-to tool for a personalized music experience tailored to the current weather conditions. It seamlessly integrates Spotify data with real-time weather information, ensuring to get the perfect soundtrack for any climate.

## Features

1. **Data Retrieval and Preprocessing:**
   - Fetch and process the Spotify favorite songs playlist using BeautifulSoup.
   - Create a comprehensive DataFrame with song names, dance values, energy values, and happiness values.
   - Handle empty values with preprocessing techniques, ensuring data consistency.

2. **Weather Information:**
   - Retrieve current weather conditions using OpenWeatherMap API.
   - Visualize temperature, cloudiness, and humidity features through bar graphs.
   - Experience current geographical location's weather map come alive using folium.

3. **Dynamic Song Selection Algorithm:**
   - Formulate an algorithm summing dance, energy, and happiness values.
   - Dynamically select songs based on the current temperature:
     - Below 0°C: Algorithm summation between 0-100.
     - 0-20°C: Algorithm summation between 100-200.
     - Above 20°C: Algorithm summation above 200.
   - Display track numbers for each temperature type, providing insights into your optimal music choices.

4. **Extreme Condition Filtering:**
   - Filter based on cloudiness: If below 50%, select songs with dance values above 50.
   - Filter based on humidity: If above 70%, opt for songs with happiness values below 50.

5. **Visualization for User Understanding:**
   - Engage with bar graphs visualizing weather features, making it easy to grasp current conditions.
   - Explore the local weather map through folium, adding a spatial context to your weather experience.
   - Enjoy dynamically displayed song recommendations, providing a visual representation of user's music journey.
     
## Progress Steps of the Program

1. **Data Retrieval and DataFrame Creation:**
   - Successfully obtained and processed Spotify favorite songs playlist data.
   - Created a structured DataFrame with key song attributes.
   - Implemented preprocessing to handle empty values, ensuring data integrity.

2. **Weather API Integration:**
   - Utilized OpenWeatherMap API to retrieve real-time weather conditions.
   - Visualized weather features through bar graphs, providing an easy-to-understand overview.
   - Enhanced geographical understanding with a weather map generated using folium.

3. **Algorithm Development:**
   - Formulated an algorithm summing dance, energy, and happiness values.
   - Implemented dynamic song selection based on temperature conditions, catering to varied weather preferences.
   - Displayed track numbers for each temperature type, facilitating user exploration.

4. **Extreme Condition Filtering:**
   - Implemented filtering based on cloudiness and humidity, refining song choices for extreme conditions.
   - Visualized extreme condition checks to enhance transparency and user understanding.

## Findings

- Identified potential limitations, including the reliance on Spotify playlist data and weather API accuracy.
- Recognized the sensitivity of the algorithm to external factors like sudden weather changes.
- Modified song recommendations for extreme conditions of the weather depended on humidity and cloudiness percentages besides the temperature value.


## Limitations

- The program's reliance on Spotify playlist data may affect the diversity of song recommendations.
- The generalization of music preferences based on weather conditions may not align with individual tastes.

## Future Improvements

- Diversify data sources to enrich the playlist and enhance song recommendations.
- Introduce a user feedback mechanism to continuously improve the recommendation algorithm.
- Explore real-time data streaming for the most up-to-date weather information.

## How to Use

1. Install necessary dependencies: `pip install pandas matplotlib folium`.
2. Run the program: `CS210_TERM_PROJECT.ipynb`.
3. Follow the prompts to explore weather-based song recommendations.

### More information can be found in the presentaion pdf that is uploaded in this repistory.

## Prerequisites

Before running the analysis, make sure you have the following dependencies installed:

- Python
- Pandas
- Matplotlib
- Counter
- Reguests
- json
- os
- folium




