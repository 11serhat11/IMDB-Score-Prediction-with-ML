# IMDB-Score-Prediction-with-ML
IMDB Score Prediction with ML

#### Libraries :

- Sklearn
- Pandas
- Matplotlib
- Numpy

# Methods

### Supervised Method
![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/4.png)

### Attributes
![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/5.png)

# Testing

Testing movies that is outside of the dataset. To test movies for your own, you should enter the code below :

### Code

genre_encoder = ct.named_transformers_['encoder']

genre_features = genre_encoder.transform([['genre']]).toarray()

features = np.concatenate((genre_features, np.array([[year, duration, votes, budget, domestic, worldwide, metescore]])), axis=1)  # these are the values for the other features of the movie

prediction = regressor.predict(features)[0]

print("Predicted Value:",prediction)

#### When we execute this code for specific movies, we get this result :

#### Harry Potter :

![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/6.png)

#### Dedective Pikachu :

![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/7.png)

# Graphs

### Scatter Plot

After training the model:

![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/1.png)

### Residuals

It shows the difference between the predicted value and the true value
![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/2.png)
![Project Screenshot](https://github.com/11serhat11/IMDB-Score-Prediction-with-ML/blob/master/images/3.png)

