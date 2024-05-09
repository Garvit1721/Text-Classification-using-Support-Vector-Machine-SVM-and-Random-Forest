## Text Classification using Support Vector Machine (SVM) and Random Forest

### Description

This script performs text classification on airline sentiment data using Support Vector Machine (SVM) and Random Forest classifiers. The dataset consists of text data and corresponding sentiment labels, which are used to train the classifiers. The trained models are then evaluated on a test dataset to measure their performance.

### Data Loading and Preprocessing

The script loads the dataset from a CSV file and preprocesses the text data by tokenizing, lemmatizing, and removing stopwords, punctuation, emojis, links, and numbers. The cleaned text data is then converted into numerical features using CountVectorizer, which converts text documents into a matrix of token counts.

### Model Training and Evaluation

Two classifiers, SVM and Random Forest, are trained on the numerical features extracted from the text data. The models are trained using the fit method and evaluated using the score method. The performance of each model is measured by its accuracy on the training data.

### Prediction

The trained models are used to predict the sentiment labels for a test dataset. The predictions are compared with the labels provided by an external source to measure the accuracy of the models on unseen data.

### Hyperparameter Tuning

Hyperparameter tuning is performed on the SVM classifier using the GridSearchCV function from scikit-learn. The best hyperparameters are selected based on cross-validation performance, and the tuned model is evaluated on the test data.

