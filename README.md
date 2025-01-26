# Movie Recommendation Web App

## Project Overview
This project is a **Movie Recommendation Web App** that uses **Machine Learning** to provide personalized movie suggestions. The system leverages two types of filtering techniques to cater to different user scenarios:

1. **Content-Based Filtering**: Recommends movies to new users based on the movie's attributes (e.g., genre, cast, description).
2. **Collaborative Filtering**: Suggests movies to existing users based on ratings and preferences of similar users, using the **K-Nearest Neighbors (KNN)** algorithm.

---

## Features
- **Dynamic Recommendations**:
  - Content-based recommendations for new users.
  - Collaborative-based recommendations for existing users.
- **User-Friendly Interface**:
  - Simple and clean web interface for browsing recommendations.
- **Customizable Suggestions**:
  - Filter movies by genres, ratings, or user preferences.
- **Real-Time Updates**:
  - Reflects changes as user preferences are added or modified.

---

## Technologies Used

### Backend
- **Flask**: Python framework to handle API and server-side logic.
- **Pandas**: Data manipulation and preprocessing.
- **Scikit-learn**: Implementing machine learning algorithms (KNN).

### Frontend
- **HTML/CSS**: Structuring and styling the web pages.
- **JavaScript**: Enhancing interactivity.

### Database
- **MongoDB**: Storing user data, ratings, and movie details.

---

## Dataset
The app uses the `user_ratings.csv` dataset, which contains the following columns:
- `user_id`: Unique identifier for each user.
- `movie_id`: Unique identifier for each movie.
- `rating`: The rating given by a user to a movie (on a scale of 1-5).
- `movie_name`: The name of the movie.

The dataset has been verified for completeness, with no null or missing values.

---

## Installation Guide

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-app.git
   cd movie-recommendation-app
   ```

2. **Set Up a Virtual Environment** (Optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Start the Flask Server**:
   ```bash
   python app.py
   ```

5. **Access the Web App**:
   Open your browser and go to: `http://127.0.0.1:5000/`

---

## Usage Guide

### For New Users:
1. Enter your preferences such as favorite genres or keywords.
2. Get movie recommendations based on your inputs.

### For Existing Users:
1. Log in to the system.
2. View personalized recommendations based on your rating history.

---

## Machine Learning Approach

### Content-Based Filtering:
- Extracts key features (genres, description, etc.) from movies.
- Computes similarity scores between movies using **TF-IDF** and **Cosine Similarity**.
- Recommends movies with the highest similarity to user preferences.

### Collaborative Filtering:
- Uses the **K-Nearest Neighbors (KNN)** algorithm to find users with similar rating patterns.
- Recommends movies that similar users have liked.

---

## Future Enhancements
- Integrating **Hybrid Filtering** to combine the strengths of content-based and collaborative filtering.
- Adding **Deep Learning Models** for improved recommendations.
- Implementing **user authentication** for secure logins.
- Supporting real-time updates for new movies and ratings.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---
