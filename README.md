**Movie Recommendation System with Matrix Factorization**

This project implements a collaborative filtering-based movie recommendation system using matrix factorization with PyTorch. The system is trained on user-movie interaction data, where it predicts movie ratings by leveraging latent factor models. It’s ideal for recommending movies based on user preferences and previous ratings.
The goal of this project is to predict movie ratings by learning latent factors for users and items (movies) using matrix factorization. The project leverages PyTorch’s Embedding layer for building latent factor models and implements training loops to optimize the model on the user-movie rating dataset.

**Features :**
Matrix Factorization Model: Uses PyTorch to build a recommendation model based on matrix factorization.
Collaborative Filtering: Leverages user-item interactions to make personalized movie recommendations.
Training with GPU: Detects if GPU is available and leverages CUDA for faster training.
Dataset

This project uses the MovieLens dataset provided by Kaggle, containing user ratings on movies. Ensure the dataset has the following structure:

movies.csv: Contains movie metadata, including titles.
ratings.csv: Contains user ratings for each movie along with timestamps.

Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/yourprojectname.git
cd yourprojectname
Install the required libraries:

bash
Copy code
pip install -r requirements.txt
Usage
Load the Data: The dataset is loaded from the movies.csv and ratings.csv files.
Model Initialization: The MaxFactorization class defines the matrix factorization model with Embedding layers for users and movies.
Training: The model is trained using MSE loss and Adam optimizer, with an option to run on a GPU if available.
Prediction: After training, the model can predict movie ratings for user-movie pairs.

Results
The trained model provides movie recommendations by predicting ratings, allowing users to view a list of top recommendations based on their previous interactions.

