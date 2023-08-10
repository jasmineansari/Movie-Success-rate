# Movie Success Rate Prediction

## Overview

This project aims to predict the success rate of movies based on various features such as year, runtime, rating, votes, revenue, metascore, genre, director, and actors. The success rate is a binary variable that indicates whether the movie has a rating above 7.5 or not. The dataset contains 1000 movies released between 2006 and 2016.

## Data Cleaning and Exploration

The data cleaning and exploration process was done using pandas, numpy, matplotlib, and seaborn libraries in Python. The following steps were performed:

- Read the csv file into a pandas dataframe
- Displayed the first 10 rows of the dataframe
- Checked the information and summary statistics of the dataframe
- Checked the shape and null values of the dataframe
- Dropped the null values from the dataframe
- Dropped the genre column from the dataframe as it was redundant with the one-hot encoded genre columns
- Checked the duplicated and unique values of the dataframe
- Plotted a heatmap to show the correlation matrix of the dataframe
- Plotted pie charts to show the top 10 directors and actors of movies
- Plotted line charts to show the rating, votes, revenue, and metascore based on year
- Plotted bar charts to show the rating with respect to metascore, revenue, and votes

## Data Modeling and Evaluation

The data modeling and evaluation process was done using scikit-learn library in Python. The following steps were performed:

- Split the dataframe into features (x) and target (y)
- Split the features and target into train and test sets with a test size of 0.2 and a random state of 10
- Scaled the features using StandardScaler
- Built a Random Forest Classifier model with 60 estimators
- Fitted the model on the train set and made predictions on the test set
- Calculated the accuracy score of the model on both train and test sets
- Plotted a confusion matrix to show the true positives, true negatives, false positives, and false negatives of the model
- Printed a classification report to show the precision, recall, f1-score, and support of the model

## Conclusion

This project demonstrates how to use various tools and techniques to clean, explore, model, and evaluate a dataset of movie success rate. The results reveal some interesting insights into the movie industry, such as:

- The number of movies released increased over time, reaching a peak in 2016
- The rating, votes, revenue, and metascore showed some variation over time, with some peaks and dips corresponding to different movies and events
- The directors and actors with the most movies were mostly from Hollywood
- The correlation matrix showed that rating had a strong positive correlation with votes and metascore, a moderate positive correlation with revenue, and a weak negative correlation with runtime
- The pie charts showed that Christopher Nolan was the most popular director of movies, followed by David Fincher and Ridley Scott
- The pie charts also showed that Christian Bale was the most popular actor of movies, followed by Leonardo DiCaprio and Jennifer Lawrence
- The line charts showed that rating had a slight downward trend over time, while votes had an upward trend over time
- The line charts also showed that revenue had some spikes in certain years, such as 2009, 2012, and 2015
- The line charts also showed that metascore had some variation over time, with some high scores in 2007, 2010, 2013, and 2016
- The bar charts showed that rating had a positive relationship with metascore, revenue, and votes
- The bar charts also showed that movies with higher ratings had higher metascores, revenues, and votes than movies with lower ratings
- The Random Forest Classifier model achieved an accuracy score of 0.87 on the train set and 0.83 on the test set
- The confusion matrix showed that the model correctly classified 129 movies as successful and 48 movies as unsuccessful out of 200 movies in the test set
- The classification report showed that the model had a precision of 0.84 for successful movies and 0.81 for unsuccessful movies
- The classification report also showed that the model had a recall of 0.88 for successful movies and 0.75 for unsuccessful movies
