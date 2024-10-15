A type of regression model that predicts a probability. Logistic regression models have the following characteristics:
The label is categorical. The term logistic regression usually refers to binary logistic regression, that is, to a model that calculates probabilities for labels with two possible values. A less common variant, multinomial logistic regression, calculates probabilities for labels with more than two possible values.
The loss function during training is Log Loss. (Multiple Log Loss units can be placed in parallel for labels with more than two possible values.)
The model has a linear architecture, not a deep neural network. However, the remainder of this definition also applies to deep models that predict probabilities for categorical labels.
For example, consider a logistic regression model that calculates the probability of an input email being either spam or not spam. 
During inference, suppose the model predicts 0.72. Therefore, the model is estimating
A 72% chance of the email being spam.
A 28% chance of the email not being spam
A logistic regression model uses the following two-step architecture:
The model generates a raw prediction (y') by applying a linear function of input features.
The model uses that raw prediction as input to a sigmoid function, which converts the raw prediction to a value between 0 and 1, exclusive.
logistic regression model predicts a number. However, this number typically becomes part of a binary classification model as follows:
If the predicted number is greater than the classification threshold, the binary classification model predicts the positive class.
If the predicted number is less than the classification threshold, the binary classification model predicts the negative class.
