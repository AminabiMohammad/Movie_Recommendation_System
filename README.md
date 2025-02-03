# **Movie Recommendation System**

## **📚 Project Overview**

This project **Movie Recommendation System** uses **Content-Based Filtering (CB)** to recommend movies based on user preferences. Built with **Python** and **JavaScript**, the system leverages **TF-IDF (Term Frequency-Inverse Document Frequency)** for feature extraction and **Cosine Similarity** for calculating the similarity between movies.

## **💡 Features**

- **Content-Based Filtering:** Recommends movies similar to a user-provided movie.
- **TF-IDF Vectorization:** Converts text data into a numerical vector representation.
- **Cosine Similarity:** Computes similarity between movie vectors based on their content.

### **For Users:**
- Enter a movie name to get recommendations based on similar movies in the dataset.
- If an invalid movie name is entered, suggestions for similar movie titles are displayed.

### **Technologies Used:**
- **Python (Flask):** Backend development and recommendation logic.
- **JavaScript:** Frontend logic for handling invalid input and returning similar movie names.
- **scikit-learn:** Used for feature extraction (TF-IDF) and computing Cosine Similarity.
- **HTML:** Display of movie recommendations.

## **📊 Dataset**
- **TMDB 5000**: A dataset containing information about movies, including genres, keywords, cast, and crew.

## **🔧 Feature Extraction and Distance Metrics**

- **Feature Extraction (TF-IDF):** Converts text-based information into a vector form to represent documents. This method is used to create a "soup" of features for each movie.
- **Cosine Similarity:** Measures the similarity between two vectors by calculating the cosine of the angle between them, helping identify similar movies.
