# 🎬 Movie Recommender System

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

An interactive, content-based movie recommendation engine deployed as a web application using **Streamlit**. This system analyzes high-dimensional text data using Natural Language Processing (NLP) to find structural similarities between movies and seamlessly integrates the **TMDB API** to dynamically fetch and render movie posters.

---

## ✨ Features

* **Intelligent Recommendations:** Suggests 5 highly relevant movies based on a user's selection.
* **Content-Based Filtering:** Utilizes **Bag-of-Words** vectorization and **Cosine Similarity** to match movie metadata (genres, keywords, cast, and crew).
* **NLP Processing:** Employs **NLTK stemming** to normalize text data and improve recommendation accuracy.
* **Dynamic UI:** A clean, responsive frontend built with Streamlit that displays movie titles alongside their official posters fetched in real-time.

---

## 🛠️ Tech Stack

*   **Core Language:** `Python`
*   **Frontend Framework:** `Streamlit`
*   **Machine Learning & Data Processing:** `scikit-learn`, `NLTK`, `Pandas`, `NumPy`
*   **External API:** `TMDB (The Movie Database) API`

---

## 🧠 How It Works

1. **Data Preprocessing:** Movie tags and overviews are consolidated and processed. NLTK is used to stem words (e.g., converting "running" and "runs" to "run") to reduce dimensionality.
2. **Vectorization:** The text data is converted into vectors using a Bag-of-Words approach, ignoring common stop words.
3. **Similarity Calculation:** The distance between vectors is computed using Cosine Similarity. Movies with the highest similarity scores to the selected movie are identified as recommendations.
4. **API Integration:** The TMDB API is queried using the recommended movie IDs to fetch the corresponding high-quality poster images for the frontend.

---

## 🚀 Installation & Setup

Follow these steps to run the project locally on your machine.

### 1. Clone the repository
```bash
git clone [https://github.com/Divyanshu10045/movie-recommender-system-.git](https://github.com/Divyanshu10045/movie-recommender-system-.git)
cd movie-recommender-system
```

### 2. Create a Virtual Environment (Optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Get a TMDB API Key
* Create an account at [The Movie Database (TMDB)](https://www.themoviedb.org/).
* Navigate to your account settings and generate an API key.
* Replace the placeholder API key in the code (usually in a `.env` file or directly in the fetch function) with your unique key.

### 5. Run the Application
```bash
streamlit run app.py
```

---

## 🤝 Acknowledgments

* Data provided by [Kaggle TMDB 5000 Movie Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata) (or specify your dataset source).
* Movie posters and metadata fetched via the [TMDB API](https://www.themoviedb.org/documentation/api).
