# 🎬 Movie Recommendation System

A **Content-Based Movie Recommendation System** built using **Python and Machine Learning** techniques.
The system recommends movies similar to a movie selected by the user based on textual features such as genres, keywords, cast, tagline, and director.

This project demonstrates **Natural Language Processing (NLP)** techniques and **Cosine Similarity** to recommend movies based on similarity scores.

---

# 📌 Project Overview

Recommender systems are widely used in platforms like streaming services and e-commerce applications to provide personalized suggestions.

This project builds a **content-based filtering recommendation system** that suggests movies similar to the one entered by the user.

The system works by:

1. Extracting important movie features
2. Converting text data into numerical vectors
3. Calculating similarity between movies
4. Recommending the most similar movies

---

# ⚙️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

Libraries used:

* pandas
* numpy
* sklearn
* difflib

---

# 📂 Dataset

The dataset contains movie information including:

* Movie title
* Genres
* Keywords
* Tagline
* Cast
* Director

Example dataset columns:

```
index
title
genres
keywords
tagline
cast
director
```

---

# 🧠 Machine Learning Approach

This project uses a **Content-Based Filtering Approach**.

Steps followed:

### 1. Importing the Dependencies

Import required libraries such as pandas, numpy, and sklearn.

### 2. Data Collection and Preprocessing

Load the dataset and inspect the structure.

### 3. Loading the Data

Load the dataset from a CSV file into a Pandas DataFrame.

### 4. Data Exploration

Display the first 5 rows of the dataset.

```
movies_data.head()
```

### 5. Dataset Shape

Check number of rows and columns.

```
movies_data.shape
```

### 6. Selecting Relevant Features

The following features are used for building recommendations:

* genres
* keywords
* tagline
* cast
* director

### 7. Handling Missing Values

Replace missing values with empty strings.

```
movies_data.fillna('', inplace=True)
```

### 8. Combining Selected Features

Merge all important textual features into a single column.

Example:

```
combined_features = genres + keywords + tagline + cast + director
```

### 9. Converting Text Data into Feature Vectors

Use **TF-IDF Vectorization** to convert text data into numerical feature vectors.

### 10. Calculating Similarity

Compute similarity between movies using **Cosine Similarity**.

Cosine similarity measures how similar two vectors are based on their direction.

### 11. Taking User Input

The user enters a movie name.

Example:

```
movie_name = input("Enter your favourite movie name: ")
```

### 12. Finding Similar Movies

The system finds movies with the highest similarity scores.

### 13. Displaying Recommended Movies

The system prints the top recommended movies based on similarity.

Example output:

```
Movies Suggested for you:

1. The Dark Knight
2. Batman Begins
3. The Dark Knight Rises
4. Man of Steel
5. Watchmen
```

---

# 📊 Workflow of the Project

```
Dataset
   ↓
Data Cleaning
   ↓
Feature Selection
   ↓
Feature Combination
   ↓
TF-IDF Vectorization
   ↓
Cosine Similarity
   ↓
Movie Recommendation
```

---

# 🚀 How to Run the Project

### Step 1

Clone the repository

```
git clone https://github.com/yourusername/movie-recommendation-system.git
```

### Step 2

Install required libraries

```
pip install pandas numpy scikit-learn
```

### Step 3

Run the notebook

```
Movie_Recommendation_System.ipynb
```

### Step 4

Enter your favourite movie name to get recommendations.

---

# 📁 Project Structure

```
movie-recommendation-system
│
├── dataset
│   └── movies.csv
│
├── notebooks
│   └── movie_recommendation_system.ipynb
│
├── README.md
│
└── requirements.txt
```

---

# 📈 Future Improvements

Possible improvements to the system:

* Build a web application using Flask or FastAPI
* Add collaborative filtering
* Implement deep learning recommendation models
* Deploy the system using Docker
* Create a user interface

---

# 💡 Applications

Movie recommendation systems are used in platforms such as:

* Streaming services
* Online movie platforms
* Entertainment recommendation engines

---

# 📜 License

This project is open-source and available for learning purposes.

---

# 👨‍💻 Author

Nagaraj K
Machine Learning Engineer

GitHub: [https://github.com/knagaraj-2106](https://github.com/knagaraj-2106)

