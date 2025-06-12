
# E-Commerce Recommendation System with Flask and Machine Learning

This repository contains the code and instructions to build an E-Commerce Recommendation System using Flask and various machine learning techniques, including content-based filtering, collaborative filtering, hybrid models, and multi-model approaches. The project integrates the recommendation system with a Flask-based web application to create a seamless, personalized shopping experience.

---

## Features
- **Content-Based Filtering:** Recommends products similar to the ones a user has interacted with based on product attributes.
- **Collaborative Filtering:** Utilizes user behavior (ratings, interactions) to predict preferences.
- **Hybrid Models:** Combines multiple recommendation techniques to improve accuracy and diversity.
- **Multi-Model Recommendations:** Integrates different machine learning models to cater to diverse user preferences.
- **Flask Integration:** Includes user registration, product browsing, and dynamic recommendations on an e-commerce platform.
- **User Feedback:** Allows users to provide feedback (ratings/likes) for better personalization.

---
[Watch the UI walkthrough video](https://drive.google.com/file/d/1qSKUozX-4V9bNYzt5mXvkrQxwNingvZv/view?usp=sharing)



## Prerequisites
Ensure the following tools and libraries are installed:
- **Python 3.8+**
- Flask
- NumPy
- pandas
- scikit-learn
- TensorFlow/Keras
- matplotlib (for visualization)
- SQLAlchemy (for database integration)
- Jupyter Notebook (optional, for prototyping)

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/E-Commerce-Recommendation-System.git
   cd E-Commerce-Recommendation-System
   ```
2. **Set Up a Virtual Environment**

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. **Install Dependencies**

```bash

pip install -r requirements.txt
```
## Prepare the Dataset

Add your e-commerce dataset (products, user ratings, interactions) to the data/ directory.
Ensure the dataset includes attributes like product IDs, user IDs, ratings, and product features.
Steps to Build the Recommendation System
1. **Data Preprocessing**
Load the dataset using pandas and clean it (handle missing values, normalize features).
Create a data split for training, validation, and testing.
2. **Content-Based Filtering**
Use product features (e.g., category, brand, description) to calculate item similarity.
Implement a cosine similarity model to recommend similar items.
3. **Collaborative Filtering**
Apply matrix factorization techniques (e.g., Singular Value Decomposition) or neighborhood-based methods.
Train the collaborative filtering model using user-item interaction data.
4. **Hybrid Model**
Combine content-based and collaborative filtering predictions.
Use weighted averages or meta-models to blend the results.
5. **Multi-Model Approach**
Train multiple models for different recommendation strategies (e.g., trending items, new arrivals).
Ensemble predictions to diversify recommendations.
6. **Model Evaluation**
Evaluate the models using metrics like precision, recall, F1 score, and mean average precision (MAP).
Optimize hyperparameters for better performance.
##Integrating with Flask
1. **Set Up the Flask Application**
- Initialize a Flask project structure.
- Configure database integration using SQLAlchemy.

2. **Add Routes**
Implement routes for user registration, login, browsing, and viewing recommendations.
Example: /recommendations for serving personalized suggestions.
3. **Dynamic Recommendation Display**
Use Jinja2 templating to display personalized product cards (images, prices, ratings).
4. **User Interaction**
- Allow users to rate products or mark them as favorites.
- Store feedback for model retraining.
- Running the Application
- Start the Flask Server

```bash
flask run
```
## Access the Web Application
Open a browser and navigate to http://127.0.0.1:5000.
## Future Enhancements
- Include real-time recommendations using streaming data.
- Add advanced NLP models for product description analysis.
- Optimize for deployment on cloud platforms like AWS, Azure, or Google Cloud.
- Implement advanced feedback systems for continuous learning.
