![banner](https://github.com/PJURC-data-analysis/spotify-top-tracks/blob/main/media/banner.png)

# Spotify Top Tracks Analysis (2020)
[View Notebook](https://github.com/PJURC-data-analysis/spotify-top-tracks/blob/main/notebooks/spotify-top-tracks.ipynb)

An exploratory data analysis of Spotify's top 50 tracks from 2020, investigating the musical characteristics that contribute to a song's commercial success. This analysis uses correlation methods to identify key musical elements that are common among hit songs, providing insights for music producers and industry professionals.

## Overview

### Business Question
What musical elements are most strongly associated with hit songs on Spotify, and how can these insights inform music production decisions?

### Key Findings
- **Genre Impact**: Pop music maintains its commercial dominance, suggesting its formula resonates strongly with current listeners
- **Danceability**: High danceability scores are consistently present in top-performing tracks
- **Sound Engineering Insights**: Strong positive correlation between energy and loudness, although loudness should not be overdone
- **Production Focus**: Low instrumentality scores suggest vocal-driven tracks perform better commercially, particularly in Pop and Hip-Hop genres

### Impact/Results
- Identified specific audio feature ranges that characterize successful tracks
- Mapped genre-specific patterns in successful songs
- Created a data-driven framework for evaluating commercial potential of tracks

## Data

### Source Information
- Dataset: Spotify Top 50 Tracks 2020
- Source: [Kaggle Dataset](https://www.kaggle.com/datasets/atillacolak/top-50-spotify-tracks-2020)
- Time Period: 2020 Calendar Year

### Variables Analyzed
#### Audio Features (Spotify API Metrics)
- **Primary Metrics:**
  - Danceability (0-1): How suitable a track is for dancing
  - Energy (0-1): Perceptual measure of intensity and activity
  - Loudness (dB): Overall loudness of a track
- **Secondary Metrics:**
  - Instrumentalness (0-1): Predicts whether a track contains no vocals
  - Valence (0-1): Musical positiveness conveyed by a track
  - Acousticness (0-1): Confidence measure of acoustic sound
  - Additional: duration_ms, liveness, speechiness, tempo

#### Categorical Data
- Artist, Track Name, Album, Genre, Key

## Methods

### Analysis Approach
  - Artist
  - Album
  - Danceability
  - Loudness
  - Track Length
  - Genres
  - Correlation Analysis

### Tools Used
- Python (Data Analysis)
  - Pandas: Data manipulation and analysis
  - NumPy: Numerical computations

## Getting Started

### Prerequisites
```python
matplotlib==3.9.3
numpy==2.2.0
pandas==2.2.3
seaborn==0.13.2
```

### Installation & Usage
```bash
git clone git@github.com:PJURC-data-analysis/spotify-top-tracks.git
cd spotify-top-tracks
pip install -r requirements.txt
jupyter notebook "Spotify Top Tracks.ipynb"
```

## Project Structure
```
coursera-analysis/
│   README.md
│   requirements.txt
│   Spotify Top Tracks.ipynb
└── data/
    └── spotify_top_tracks.csv
```

## Strategic Recommendations
1. Consider the elements of the Pop genre, as its formula is still popular among listeners.
2. Make sure the song is danceable; A high rating is prevalent in the charts.
3. For added energy, consider adding more loudness, but don't overdo it.
4. Instrumentality is not a must-have for a hit song. Electronic music and vocal-driven Hip-Hop/Rap score high in danceability

## Future Improvements
1. Additional Numeric Variables
   * Tempo - BPM of the song
   * Lyrical complexity score

2. Additional Analysis
   * Gender influence in specific genre success
   * Most successful sub-genres of pop

3. Dataset Extensions
   * Top 100 charts
   * Charts by region / continent

## Acknowledgments
- Kaggle for dataset provision
- Spotify for the top tracks listing