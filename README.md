# temperature_playlist_analyzer
A Spotify Playlist Analyzer for Weather Condition

# Spotify Weather-Based Music Recommender

## Overview

This Python program, dubbed **Spotify Weather-Based Music Recommender**, is your go-to tool for a personalized music experience tailored to the current weather conditions. It seamlessly integrates Spotify data with real-time weather information, ensuring you get the perfect soundtrack for any climate.

## Features

1. **Data Retrieval and Preprocessing:**
   - Fetch and process your Spotify favorite songs playlist using BeautifulSoup.
   - Create a comprehensive DataFrame with song names, dance values, energy values, and happiness values.
   - Handle empty values with preprocessing techniques, ensuring data consistency.

2. **Weather Information:**
   - Retrieve current weather conditions using OpenWeatherMap API.
   - Visualize temperature, cloudiness, and humidity features through bar graphs.
   - Experience your geographical location's weather map come alive using folium.

3. **Dynamic Song Selection Algorithm:**
   - Formulate an algorithm summing dance, energy, and happiness values.
   - Dynamically select songs based on the current temperature:
     - Below 0°C: Algorithm summation between 0-100.
     - 0-20°C: Algorithm summation between 100-200.
     - Above 20°C: Algorithm summation above 200.
   - Display track numbers for each temperature type, giving you insights into your optimal music choices.

4. **Extreme Condition Filtering:**
   - Filter based on cloudiness: If below 50%, select songs with dance values above 50.
   - Filter based on humidity: If above 70%, opt for songs with happiness values below 50.

5. **Visualization for User Understanding:**
   - Engage with bar graphs visualizing weather features, making it easy to grasp current conditions.
   - Explore your local weather map through folium, adding a spatial context to your weather experience.
   - Enjoy dynamically displayed song recommendations, providing a visual representation of your music journey.

## Limitations

- The program's reliance on Spotify playlist data may affect the diversity of song recommendations.
- The generalization of music preferences based on weather conditions may not align with individual tastes.

## Future Improvements

- Diversify data sources to enrich the playlist and enhance song recommendations.
- Introduce a user feedback mechanism to continuously improve the recommendation algorithm.
- Explore real-time data streaming for the most up-to-date weather information.

## How to Use

1. Install necessary dependencies: `pip install pandas matplotlib folium`.
2. Run the program: `python main.py`.
3. Follow the prompts to explore weather-based song recommendations.



