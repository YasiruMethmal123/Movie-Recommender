#** 🎬 Movie Recommender System**

This repository contains a Movie Recommendation System built with Python, Streamlit, and machine learning techniques. The system suggests movies similar to a user-selected title by analyzing similarity scores and fetching movie posters using the TMDB API.

📂 Project Structure
├── app.py                     # Streamlit web app for recommendations
├── MovieRecommender.ipynb     # Jupyter Notebook for model training & exploration
├── model/
│   ├── movie_list.pkl         # Preprocessed movie metadata
│   └── similarity.pkl         # Precomputed similarity matrix
└── README.md                  # Project documentation

##**🚀 Features**

- Interactive Web App (Streamlit)
- Search for a movie and get 5 recommendations.
- Displays movie posters using TMDB API.
- Content-Based Recommendation
- Uses cosine similarity on movie metadata.
- Trained and processed in the provided Jupyter Notebook.
- Poster Fetching
- Dynamically retrieves posters from The Movie Database (TMDB).

##**⚙️ Installation**

**Clone the repository:**

git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender


**Create and activate a virtual environment:**

python -m venv venv
source venv/bin/activate    # On Linux/Mac
venv\Scripts\activate       # On Windows


**Install dependencies:**

pip install -r requirements.txt

**▶️ Usage**
Run the Streamlit app:
streamlit run app.py


**Select a movie from the dropdown.**

**Click Show Recommendation.**

**View top 5 recommended movies with posters.**

**Explore in Jupyter Notebook:**
- jupyter notebook MovieRecommender.ipynb

##**🛠️ Requirements**

- Python 3.8+
- Streamlit
- Pandas
- Scikit-learn
- Requests
- Pickle

(See requirements.txt for full dependencies.)

##**🔑 API Key**

The app uses the TMDB API. Replace the placeholder API key in app.py with your own key:

url = f"https://api.themoviedb.org/3/movie/{movie_id}?api_key=YOUR_API_KEY&language=en-US"


Get your API key here: TMDB API

#**📸 Demo**

Example output:

Input Movie: The Dark Knight
Recommendations:
- Batman Begins
- The Dark Knight Rises
- Inception
- Man of Steel
- Joker


(Each result is shown with its poster in the Streamlit app.)

📚 Acknowledgments

The Movie Database (TMDB)
 for movie metadata & posters.

Streamlit for interactive web app framework.
