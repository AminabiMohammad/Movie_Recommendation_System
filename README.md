Movie Recommendation System:
This Content Based Filtering Movie Recommender is built on a Flask app using Python and JavaScript. Two code snippets demonstrate the concept of Content-Based (CB) filtering. The first snippet uses Python and the "scikit-learn" package, while the second snippet uses JavaScript without any packages, relying solely on logic. The recommender leverages feature extraction methods and distance metrics to generate recommendations.

Dataset: TMDB 5000

Content-Based Filtering Methods:
Feature extraction methods like TF-IDF vectorize the text data, and distance metrics like Cosine Similarity compute the similarity between each item by calculating the distance between vectors.

Feature Extraction Method:
The feature extraction method used in this recommender is Term Frequency-Inverse Document Frequency (TF-IDF). TF-IDF converts textual information into a Vector Space Model (VSM), an algebraic model representing text documents as vectors, also known as index terms. In CB filtering, a multi-dimensional vector represents user preferences and available items, with each item stored as a vector of its features. The angles between these vectors are useful for calculating similarity between items.

Distance Metric:
The distance metric used in this recommender is Cosine Similarity. Cosine Similarity measures the cosine of the angle between two vectors projected in a multidimensional vector space. It considers non-binary vector values, focusing on the contents of the items and disregarding their size, making it suitable for text documents with different word counts.

Code Snippets:
Two code snippets demonstrate the use of TF-IDF and Cosine Similarity in generating recommendations.

Python Code:
The Python code in app.py generates a list of movie recommendations based on a valid movie name entered by the user. If the entered movie name matches one in the dataset, recommendations are generated according to the 'soup' column (all details concatenated into one string) of each movie. This code uses the TF-IDF Vectorizer and Cosine Similarity functions imported from the "scikit-learn" package.

scikit-learn documentation: TF-IDF Vectorizer and Cosine Similarity

JavaScript Code:
The JavaScript code in notfound.html executes when the user enters an invalid movie name. This code returns movie titles similar to the input, if applicable. The entered data is checked against all existing movie names to find the most similar ones. Since no packages are used, a dictionary stores terms for vectorizing purposes, and several functions compute the TF-IDF and Cosine Similarity values.

Activate environment and install requirements:
1.)python -m venv venv
.\venv\scripts\activate
python -m pip install -r requirements.txt 


2.)Run Flask app:
set FLASK_APP=app.py
set FLASK_ENV=development
flask run
