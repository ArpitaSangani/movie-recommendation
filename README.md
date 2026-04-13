🎬 The Movie Cinema

A full-stack movie discovery web app that fetches real-time movie details, analyzes user sentiments from IMDB reviews, and recommends similar movies — all in one place.

📌 Overview
The Movie Cinema lets you search for any movie and instantly get:

Full movie details (poster, overview, rating, genre, release date, runtime, status)
Top cast info with bios, birthdays, and birthplaces
IMDB user reviews with sentiment analysis (Good 😄 / Bad 😟)
A list of recommended movies based on content similarity

Movie data is fetched via the TMDB API. User reviews are scraped from IMDB using BeautifulSoup4 and analyzed using a trained NLP model. Recommendations are powered by cosine similarity.

✨ Features

🔍 Smart Search — Autocomplete with typo tolerance
🎞️ Movie Details — Fetched live from TMDB API
🧑‍🎤 Cast Profiles — Photos, character names, bios & more
💬 Sentiment Analysis — Real IMDB reviews classified as Good/Bad using NLP
🤖 Content-Based Recommendations — Cosine similarity to find movies you'll love
🌐 Multi-language Support — Works for all language movies

🧠 How Recommendations Work
The recommendation engine uses content-based filtering with cosine similarity.

Each movie is represented as a vector based on its metadata (title, genre, cast, keywords, etc.)
Cosine similarity measures the angle between two vectors — the smaller the angle, the more similar the movies
The top N most similar movies to your search are returned as recommendations
