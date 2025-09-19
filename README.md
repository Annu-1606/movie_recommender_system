# 🎬 Movie Recommender App

A **movie recommendation system** built with **Streamlit** that suggests movies based on similarity. It also displays movie posters using **The Movie Database (TMDb) API**.

---

## ✨ Features

- Search for a movie using a dropdown or by typing the name.
- Get **5 movie recommendations** similar to the selected movie.
- View **movie posters** fetched dynamically from TMDb.
- Simple, interactive, and user-friendly interface.

---

## 🛠️ Technologies Used

- Python 3.x
- Streamlit
- Pandas
- Requests
- Pickle (for precomputed movie similarity data)
- TMDb API

---

## 📦 Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
Install the required packages:

bash
Copy code
pip install -r requirements.txt
Make sure you have the following files in your project:

movies_dict.pkl – Dictionary of movies.

similarity.pkl – Precomputed similarity matrix.

Run the app:

bash
Copy code
streamlit run app.py

## 🖥️ How It Works
User selects a movie from the dropdown.

The app calculates the most similar movies using a precomputed similarity matrix.

Movie posters are fetched from TMDb API using the movie IDs.

Top 5 recommended movies with their posters are displayed in columns.

## 🔑 TMDb API Key
The app uses the TMDb API to fetch movie posters. Replace the API key in the code if needed:

python
Copy code
url = "https://api.themoviedb.org/3/movie/{}?api_key=<YOUR_API_KEY>&language=en-US"
