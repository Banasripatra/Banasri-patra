🎧 Spotify Tracks EDA — Exploratory Data Analysis (Presentation Version)

📘 Overview

This project presents a detailed Exploratory Data Analysis (EDA) of the Spotify Tracks Dataset, prepared for a college presentation.
The analysis explores how different audio features such as energy, danceability, and valence influence the popularity of songs, and how music trends have changed over the years.


---

🎯 Objectives

The main objectives of this project are:

To study the distribution of major musical features like energy, valence, danceability, and popularity.

To explore relationships between song features and popularity.

To understand temporal trends in music over different decades.

To identify top artists and languages based on popularity.

To provide data-driven recommendations for predicting hit songs.



---

📊 Dataset Summary

Dataset Name: Spotify Tracks Dataset
Source: Spotify Web API / Kaggle
Total Records: Around 114,000 tracks

Key Features:

track_name: Name of the song

artist_name: Artist who performed the track

year: Year of release

popularity: Popularity score (0–100)

danceability: Rhythm and movement suitability

energy: Intensity or activity level of the track

valence: Positiveness or musical mood

acousticness: Degree of acoustic sounds

instrumentalness: Likelihood of instrumental-only music

speechiness: Amount of spoken words

tempo: Beats per minute (BPM)

duration_ms: Duration of song

language: Detected language of lyrics



---

🔍 Univariate Analysis

Popularity: Right-skewed distribution — most songs have low popularity.

Danceability: Left-skewed — most songs are rhythmic and danceable.

Energy: Concentrated near high values — modern songs are energetic.

Valence: Bimodal — happy and neutral/sad moods both common.

Duration: Mostly between 3–5 minutes.

Tempo: Two main peaks around 120 BPM and 140 BPM.



---

🔗 Bivariate Analysis

Popular songs usually have danceability above 0.4.

Shorter songs tend to perform better than longer ones.

Songs with low energy are rarely popular.

Valence (mood) does not strongly predict song success.

Energy and Loudness are highly correlated (redundant pair).



---

🧠 Correlation Insights

Feature	Correlation with Popularity

Energy	+0.15
Valence	+0.15
Danceability	+0.14
Acousticness	-0.14
Instrumentalness	-0.13


Recommendation:
Remove redundant variables such as Loudness (highly correlated with Energy).


---

📅 Temporal Trends

Energy has increased steadily since the 1970s.

Valence (positiveness) has decreased after the mid-1990s.

Danceability increased after the 1980s Disco era.

Speechiness rose in the 2020s, reflecting more rap and spoken content.

Duration has become shorter in the streaming era.



---

🌍 Language & Artist Analysis

Most popular languages:

Korean (average popularity ≈ 27.5)

Hindi (≈ 18.5)

Malayalam (lowest, ≈ 7)


Top artists by number of tracks: Shankar Mahadevan, Ramin Djawadi, Alan Silvestri.

Top artists by popularity: Rihanna, Taylor Swift, Kendrick Lamar, LE SSERAFIM.



---

💡 Key Findings

Popular songs are more energetic and danceable.

Shorter tracks tend to be more successful.

Mood alone does not decide a hit.

Modern music is more intense, less acoustic, and more rhythmic.



---

✅ Recommendations

Treat the problem as a classification task (“Hit” or “Not Hit”) instead of regression.

Remove redundant features like loudness to avoid correlation bias.

Use interaction features such as Energy × Valence to capture combined effects.

Clean data by removing instrumental-only and soundtrack entries.

Focus on temporal patterns while predicting future popularity.



---

⚙ Technical Information

Language Used: Python 3.11
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Plotly
Environment: Jupyter Notebook


---

📈 PPT Presentation Flow

1. Introduction and Objectives


2. Dataset Description


3. Univariate Analysis


4. Bivariate and Correlation Analysis


5. Temporal Trends


6. Language and Artist Insights


7. Key Findings


8. Recommendations


9. Future Work


10. Conclusion




---

🚀 Future Work

Build machine learning models to predict song popularity.

Perform lyric-based sentiment analysis.

Create interactive dashboards using Streamlit or Dash.

Apply time-series forecasting for feature trends.



---

👩‍💻 Author

Name: Banasri Patra
College: Government College of Engineering and Ceramic Technology (GCECT), Kolkata
Project Type: College Presentation on Data Analysis


---

🏁 Conclusion

This project highlights how data analysis can explain music trends and the factors influencing Spotify track popularity.
The findings show that music has evolved to become shorter, more energetic, and more dance-focused, and that data-driven insights can guide producers, analysts, and music enthusiasts alike.
