# RECOMMENDATION-SYSTEM

COMPANY NAME: CODTECH IT SOLUTIONS

NAME: DEVARASETTY SRI RANGA CHANDANA NAIDU

INTERN ID: CT06DF182

DOMIAN: MACHINE LEARNING

DURATION: 6 WEEKS

MENTOR: NEELA SANTHOSH KUMAR

PROJECT DESCRIPTION:

In today’s digital world, recommendation systems play a vital role in improving user experience by offering personalized suggestions. This project focused on building a movie recommendation system using collaborative filtering and matrix factorization techniques, implemented in Python using the Surprise machine learning library. The system predicts user preferences and recommends movies they are likely to enjoy, based on historical rating patterns from other similar users.

The goal of this project was to develop a functioning recommendation engine that demonstrates the application of machine learning in the domain of personalized content delivery. The system was built and tested using the MovieLens 100K dataset, a widely-used dataset in the field of recommender systems. This dataset contains 100,000 movie ratings (on a scale from 1 to 5) from 943 users on 1,682 movies.

The first step involved preprocessing the dataset by reading it into a pandas DataFrame and formatting it for compatibility with the Surprise library. Each row in the dataset included a user ID, item (movie) ID, rating, and timestamp. A custom reader object was defined to interpret the rating scale, and the data was loaded into a Surprise dataset object.

The collaborative filtering method used was matrix factorization via Singular Value Decomposition (SVD). SVD is a powerful technique that reduces the high-dimensional user-item matrix into two lower-dimensional matrices: one representing users and the other representing items. When multiplied together, these matrices approximate the original ratings, allowing the system to make predictions for unrated items.

The dataset was split into training and testing sets using an 80-20 split. The model was trained on the training set and evaluated on the test set using two commonly used metrics: Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE). The model achieved an RMSE of approximately 0.9372 and an MAE of around 0.7395, which indicates a reasonably good performance for a basic model without hyperparameter tuning or advanced features.

After training, the model was used to generate top-N recommendations for users. Specifically, for a given user (e.g., User 878), the model predicted ratings for movies the user had not yet seen, sorted them by predicted score, and recommended the top 5 movies. The output included predicted ratings such as 3.91, 3.82, etc., for various movie IDs. This demonstrated the model's ability to personalize content based on collaborative patterns in the data.

The project was implemented using Google Colab, which provided a cloud-based Python environment with necessary libraries and GPU support. External libraries used included scikit-surprise for model development, numpy and pandas for data processing, and wget for downloading the dataset.

This project provided a strong foundation in understanding the mechanics of recommendation systems, especially collaborative filtering and matrix factorization. It highlighted the importance of using real-world datasets and evaluation metrics to assess model performance. Additionally, it showed how even simple models can provide meaningful insights and user personalization when built correctly.

In conclusion, the recommendation system developed in this project successfully delivered personalized movie recommendations using collaborative filtering techniques. It was an excellent learning experience in machine learning, model evaluation, and data handling. With further improvements such as content-based filtering, hybrid models, or deep learning, the system could be extended for real-world production use. This project fulfills the requirements of the CodTech internship and demonstrates practical application of data science skills.

OUTPUT: Evaluation Metrics: RMSE: 0.9372 MAE: 0.7395

Top recommendations for User 878: Movie ID: 59, Predicted Rating: 3.91 Movie ID: 22, Predicted Rating: 3.82 Movie ID: 498, Predicted Rating: 3.70 Movie ID: 427, Predicted Rating: 3.66 Movie ID: 474, Predicted Rating: 3.63
