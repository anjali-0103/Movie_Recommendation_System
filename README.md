# 🎬 Movie Recommendation System

A Content-Based Movie Recommendation System built using Python, Pandas, Scikit-learn, and Natural Language Processing (NLP). This project recommends movies similar to a user's selected movie by analyzing movie metadata such as genres, keywords, cast, crew, and overview.

---

## 📌 Project Overview

The Movie Recommendation System suggests movies based on their similarity to a selected movie. It uses a **Content-Based Filtering** approach instead of collaborative filtering.

The recommendation model combines movie features into a single text column, converts the text into numerical vectors using **TF-IDF**, and calculates similarity using **Cosine Similarity**.

---

## 🚀 Features

- Content-Based Movie Recommendation
- Data Cleaning and Preprocessing
- Feature Engineering
- TF-IDF Vectorization
- Cosine Similarity Matrix
- Genre-based Movie Recommendation
- Save Model using Pickle
- Easy to Extend for Web Applications

---

## 🛠️ Technologies Used

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Pickle
- Jupyter Notebook

---

## 📂 Dataset

This project uses the **TMDB 5000 Movie Dataset**.

Dataset Files:

- tmdb_5000_movies.csv
- tmdb_5000_credits.csv

The datasets contain:

- Movie Title
- Genres
- Overview
- Keywords
- Cast
- Crew
- Popularity
- Release Date

---

## 📁 Project Structure

```
Movie-Recommendation-System/
│
├── Movie_Recommendation_System.ipynb
├── tmdb_5000_movies.csv
├── tmdb_5000_credits.csv
├── similarity.pkl
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
```

Move into the project directory

```bash
cd movie-recommendation-system
```

Install required libraries

```bash
pip install pandas numpy scikit-learn
```

Open Jupyter Notebook

```bash
jupyter notebook
```

Run all notebook cells.

---

## 📊 Workflow

### 1. Import Libraries

- Pandas
- NumPy
- Sklearn
- Pickle

### 2. Load Dataset

Read both movie and credits datasets.

### 3. Merge Dataset

Merge datasets using the movie title.

### 4. Data Cleaning

- Remove unnecessary columns
- Handle missing values
- Remove duplicates

### 5. Feature Engineering

Extract:

- Genres
- Keywords
- Cast
- Director
- Overview

Combine all into one column called **tags**.

### 6. Text Vectorization

Convert text into vectors using:

```
TF-IDF Vectorizer
```

### 7. Similarity Calculation

Compute movie similarity using:

```
Cosine Similarity
```

### 8. Recommendation

Return Top 5 most similar movies.

---

## 📌 Example

Input

```
Avatar
```

Output

```
Guardians of the Galaxy
John Carter
Star Trek
Alien
The Fifth Element
```

---

## 📈 Recommendation Function

```python
recommend("Avatar")
```

Returns a list of recommended movies based on similarity.

---

## 💾 Saving the Model

The similarity matrix is saved using Pickle.

```python
import pickle

pickle.dump(similarity, open("similarity.pkl","wb"))
```

---

## 📚 Libraries Required

```text
pandas
numpy
scikit-learn
pickle
ast
```

Install all libraries

```bash
pip install pandas numpy scikit-learn
```

---

## 🎯 Future Improvements

- Build a Streamlit Web App
- Add Movie Posters using TMDB API
- Hybrid Recommendation System
- User Authentication
- Search Suggestions
- Recommendation History

---

## 📸 Output

The system accepts a movie title as input and recommends similar movies based on content similarity.

Example:

```
Input:
Iron Man

Recommendations:
Iron Man 2
Avengers
Captain America
Thor
The Incredible Hulk
```

---

## 👨‍💻 Author

**Anjali Sharma**

Python Developer | Machine Learning Enthusiast

---

## 📄 License

This project is developed for educational and learning purposes.
