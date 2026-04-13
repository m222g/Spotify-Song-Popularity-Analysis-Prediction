# Spotify Song Popularity & Analysis

## Executive Summary
This project explores Spotify song metadata to understand if audio features can predict a song’s popularity. A machine learning model (Random Forest Classifier) was trained to categorize songs as high- or low-popularity based on musical attributes such as tempo, danceability, energy, and acousticness. The final model achieved ~77% accuracy, demonstrating that audio features have a strong ability to predict a song’s popularity. 

### Business Problem
This project aims to answer the question: Can a song’s audio features be used to predict its popularity?
Understanding this relationship helps stakeholders in the music industry (artists, producers, record label executives) make data-driven decisions about marketing and production strategies. 

### Methodology
Data Collection: Kaggle dataset [(Spotify Tracks Dataset)](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)

Data Cleaning: Preprocessed 12k+ song records

Data Preparation: Engineered target variable for high or low popularity classification using the median popularity score of 35

Data Splitting/Model Preparation: Split the data into 80% training and 20% testing

Modeling: Trained and optimized a Random Forest Classifier

Evaluation: Evaluated the model’s performance using a confusion matrix, accuracy score, and feature importance analysis

### Skills
Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)

Data Cleaning & Preprocessing

Machine Learning (Random Forest Classifier)

Feature Engineering

Model Evaluation

Data Visualization


### Results and Business Recommendations

#### Model Performance
-	Baseline Model Accuracy:  76.27%
-	Final Model Accuracy: 76.52%
-	Balanced confusion matrix with improved ability to accurately classify
-	Strong model performance above 70% accuracy benchmark

<img width="535" height="462" alt="Confusion Matrix" src="https://github.com/user-attachments/assets/4c4ce4ee-d339-4383-be63-6ddf6c90cfa0" />



#### Key Insights
-	The most influential features:
    - Duration
    - Danceability
    - Acousticness
-	Audio features show measurable impact on the predictability of song popularity

<img width="1125" height="468" alt="feature importance" src="https://github.com/user-attachments/assets/26fbd69c-2d4c-466f-9332-c4fbcf163b16" />



#### Recommendations:
1.	Artists should take advantage of the most influential features when producing songs by prioritizing duration, danceability, and acousticness
2.	Record labels can use predictive modeling to gauge a song’s success before it’s released
3.	Allocate and invest in marketing and production resources accordingly, based on predicted popularity
4.	Feature importance can guide creative decision-making in music production


### Next Steps
1.	Test additional models for best predictive power (Logistic Regression, Gradient Boosting, XGBoost)
2.	Include other external factors (artist popularity, streaming counts, social media following)
3.	Improve classification threshold (beyond splitting at the median)
4.	Build and launch the model as a web application to predict song popularity in real-time
