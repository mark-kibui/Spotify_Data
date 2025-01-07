# Spotify Data Visualizations

## Overview
This project involves exploring and visualizing Spotify's music dataset to uncover trends, insights, and patterns in the data. By leveraging visualizations, we aim to better understand the relationships between different features and their impact on music recommendations, popularity, and user preferences.

## Goals
1. **Understand Data Distribution:** Explore feature distributions such as song popularity, duration, tempo, and energy levels.
2. **Identify Relationships:** Analyze correlations between features like danceability, energy, and loudness.
3. **Highlight Patterns:** Showcase trends in music attributes over time.
4. **Provide Insights for Recommendations:** Use visualizations to support the rationale for building recommendation systems.

## Data Description
The dataset includes features extracted from Spotify tracks:
- **Track Information:** Track ID, name, and artist name.
- **Audio Features:** Danceability, energy, loudness, tempo, acousticness, instrumentalness, liveness, valence, and speechiness.
- **Popularity Metrics:** Song popularity score.
- **Temporal Data:** Release year.
- Below is a tabular representation of columns and their description

| Feature Name | Description |
| :--- | :--- |
| popularity | A measure of the song's popularity on Spotify |
| year | The year the song was released |
| genre | The primary genre of the song |
| danceability | Describes how suitable the track is for dancing |
| energy | Represents the perceived intensity and activity level of the track |
| key | The musical key of the song |
| loudness | The overall loudness of the track in decibels (dB) |
| mode | Indicates whether the track is in major (1) or minor (0) key |
| speechiness | The presence of spoken words in the track |
| acousticness | A confidence measure of whether the track is acoustic |
| instrumentalness | The presence of vocals in the track |
| liveness | A confidence measure of whether the track was performed live |
| valence | The positivity conveyed by the track |
| tempo | The average tempo of the track in beats per minute (BPM) |
| time_signature | The time signature of the track |
| duration_minutes | The duration of the track in minutes |

## Tools and Libraries
- **Python Libraries:**
  - `pandas` for data manipulation.
  - `matplotlib` and `seaborn` for visualizations.
  - `plotly` for interactive plots.

## Key Visualizations
### 1. **Feature Distributions**
- **Goal:** Understand the distribution of individual audio features.
- **Method:** Used histograms and KDE plots to visualize distributions.
- **Insights:**
  - Popular songs tend to have high danceability and energy.
  - Acousticness has a skewed distribution, indicating most songs are not acoustic.

### 2. **Correlation Heatmap**
- **Goal:** Identify relationships between numerical features.
- **Method:** Used a heatmap to visualize Pearson correlation coefficients.
- **Insights:**
  - Danceability and energy are strongly correlated.
  - Loudness has a negative correlation with acousticness.

### 3. **Trend Analysis Over Time**
- **Goal:** Examine how music features evolved over decades.
- **Method:** Line plots and scatter plots grouped by release year.
- **Insights:**
  - Loudness has steadily increased over the years.
  - Songs have become more danceable and energetic over time.

### 4. **Popularity vs. Audio Features**
- **Goal:** Determine which features influence a song’s popularity.
- **Method:** Boxplots and scatter plots of popularity scores against features.
- **Insights:**
  - Popular songs often have high valence (positivity).
  - Tempo and loudness are key factors for hit tracks.

### 5. **Genre Analysis**
- **Goal:** Explore how audio features vary across genres.
- **Method:** Bar plots and violin plots segmented by genre.
- **Insights:**
  - Classical music has high acousticness and low energy.
  - Hip-hop tracks often have high speechiness.

### 6. **Interactive Visualizations**
- **Goal:** Enable deeper exploration of individual tracks and trends.
- **Method:** Used Plotly to create interactive scatter and bar plots.
- **Features:**
  - Hover functionality for detailed track information.
  - Filters for specific genres and time ranges.

## Conclusion
The visualizations provide valuable insights into the characteristics of Spotify tracks and highlight patterns that can inform music recommendation systems. By analyzing relationships between features, trends over time, and genre-specific characteristics, this project enhances our understanding of the dataset.

## Future Work
- Add advanced visualizations like clustering plots for grouped insights.
- Explore user listening habits and preferences.
- Integrate visualizations with a recommendation engine for better context.

## How to Run
1. Clone the repository.
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook containing visualizations:
   ```bash
   jupyter notebook spotify_visualizations.ipynb
   ```
4. Explore the generated plots interactively or as static outputs.

## Examples
Below are some examples of insights:
- **Insight 1:** Danceability vs. Popularity: Songs with a danceability score above 0.7 tend to have higher popularity.
- **Insight 2:** Tempo Over Time: Tempo trends upward from the 1980s to the present, reflecting changes in music styles.

For more detailed explanations, refer to the comments within the visualization notebook.

