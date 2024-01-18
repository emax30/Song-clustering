# Unsupervised-song-clustering
Unsupervised clustering of top-100 singles of the year (1959-2022, split into three periods) based on their lyrics.

Song titles and artists of Billboard year-end hot 100 singles for years 1959-2022 were scraped from Wikipedia. The corresponding song lyrics were then scraped from Genius API (API client acccess token required) using [LyricsGenius](https://github.com/johnwmillr/LyricsGenius) by John W. Miller. The data was cleaned up, stopwords were removed and lemmatization was applied, and unsupervised k-means clustering was performed on three separate groups of songs: 1959-1980, 1981-2001, and 2002-2022. Analysis of the resulting clusters in terms of word frequency revealed tight clusters of songs with a lot of interjections ("La-la-la", "Oh-oh" etc.) and more diffuse clusters with high frequency of the word "love" in their lyrics. The clusters were also analyzed in terms of their lyrics sentiment and overall songs from 2002-2022 were found to have considerably lower vader and textblob sentiment scores (i.e the most popular songs are less cheerful today compared to several decades ago).

# Final clusters visualized
![1959-1980 clusters]()
![1981-2001 clusters](https://github.com/emax30/Song-clustering/blob/main/screenshots/Screenshot%202024-01-17%20172548.png)
![2002-2022 clusters]()
