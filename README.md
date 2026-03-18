# machine-learning-projects
This is a classic spam detector ml model that uses thge dataset:-spam_or_not_spam.csv. the model here used is logistic regression using sci-kit learn library. The repository includes data importing, cleaning, preprocessing. tf-idf vectorisation has been implemented for text to numeric conversion; along with normalisation.
LIBRARIES USED:-
PANDAS
NUMPY
MATPLOTLIB
SCI-KIT LEARN.
AN EDA on the datset was conducted which included data cleaning, removal of nulls and duplicates etc.
The text vectorisation was done to convert the text emails into numbers, then normalisation was done to balance the scales. Such that we got all unit vectors.
After that Logistic REgression model was implemented on the datset to predict whether a given email is spam or not. 
The Logistic regression uses sigmoid function for the prediction. It tries to minimize the binary cross-entropy loss for the model parameters. The library (sci-kit learn) also implements regullarization techniques to smoothen the decision boundary.
It decided the spam not spam based on a threshold probability.
Then the model's metrics were checked using the metrics package from sci-kit learn library. 
The dataset used has been attached in the repository.
