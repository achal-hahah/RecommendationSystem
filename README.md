🎬 Movie Recommender System
A content-based movie recommendation web application built with Streamlit, FastAPI, and scikit-learn, powered by movie data and images from The Movie Database (TMDB).

🚀 Features
Home Feed Discovery: Browse categories including Trending, Popular, Top Rated, Now Playing, and Upcoming.

Dynamic Search & Autocomplete: Real-time keyword search with instant title suggestions.

Detailed Movie Information: Complete view of movie posters, backdrops, genres, release dates, and story overviews.

Smart Recommendations:

Content Similarity (TF-IDF): Machine-learning-driven recommendations based on plot and metadata.

Genre-Based Recommendations: Dynamic matching for movies sharing similar genres.

Customizable Interface: Adjustable column grid density and responsive modern styling.

🛠️ Tech Stack
Frontend: Streamlit

Backend API: FastAPI, Uvicorn, HTTPX

Machine Learning & NLP: scikit-learn, Pandas, NumPy, SciPy

Data Source: TMDB API

📁 Project Structure
Plaintext
├── app.py              # Streamlit frontend client
├── main.py             # FastAPI backend service
├── requirements.txt    # Project dependencies
├── runtime.txt         # Python runtime environment version
├── df.pkl              # Preprocessed movies dataset
├── indices.pkl         # Title-to-index lookup mappings
├── tfidf.pkl           # Trained TF-IDF Vectorizer
└── tfidf_matrix.pkl    # Precomputed similarity matrix
⚙️ Installation & Local Setup
1. Clone the repository
Bash
git clone https://github.com/YOUR_GITHUB_USERNAME/RecommendationSystem.git
cd RecommendationSystem
2. Create and activate a virtual environment
Bash
# macOS/Linux
python3 -m venv .venv
source .venv/bin/activate

# Windows
python -m venv .venv
.venv\Scripts\activate
3. Install required packages
Bash
pip install -r requirements.txt
4. Start the FastAPI backend
Bash
uvicorn main:app --reload --port 8000
5. Launch the Streamlit frontend
Open a second terminal window and run:

Bash
streamlit run app.py
🌐 Deployment Details
Backend: Hosted on Render ([https://movie-rec-466x.onrender.com](https://movie-rec-466x.onrender.com)).

Frontend: Hosted on Streamlit Community Cloud.

📝 License
This project is licensed under the MIT License. Feel free to use and modify it.
