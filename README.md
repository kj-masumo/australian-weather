# autralian-weather

## Intro
This is a machine learning project that aims to try to predict whether or not it rained a measureable amount the following day given some variables about the current day. This project was mainly completed to demonstrate a basic understanding of how to use various sklearn packages to create a machine learning model as well as report and visualize some of the relevant findings. The findings themselves are secondary, as meteorologists are much better-equipped to predict weather patterns than a simple KNN model.

## Methodology
I used sklearn's train_test_split package to split the data into training and testing data, the StandardScaler package to standardize the features, and KNeighborsClassifier for the model construction and hyperparameter tuning. I then used confusion_matrix, f1_score, and accuracy_score to report on the findings and accuracy of the model.

## Findings
After tuning the hyperparameters and feature list, I found that the highest reported F1 score came from K = 7. However, the primary conclusion that I came to was that the model was not very good at predicting rain patters overall. This was partially because of the lack of complexity of the features themselves, but primarily because of the curse of dimensionality suffered by KNN models. There was simply not enough data to create an accurate model to try to predict rain patters with the given features.

## Future Work
Future work might include reworking the research question to find out which features are most predictive of rain the following day. This might retroactively help models like this one, as it might help with more precise feature selection.

## Files
* australian_weather.ipynb: The notebook file containing the walkthrough of the data cleaning, model creation, hyperparameter tuning, and results reporting
