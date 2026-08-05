## 🚀 Installation & Setup

Follow these steps to run the project locally on your machine.

### 1. Clone the repository
```bash
git clone [https://github.com/your-username/movie-recommender-system.git](https://github.com/Divyanshu10045/movie-recommender-system-.git)
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
