This is a classification problem , I wanted to try few models and compare their performance . 
I started with preprocessing the data, I used ordinal encoder on few columns from train_features dataframe and the rest I used Onehotencoder to encode the values. 
I used the Training set to train a logistic regression model . My idea is to use each target variables at once to train and get the probability of predictions on test features for each then combine the data frames . 
(I wanted to do the simple model first) then I would have progressed onto using multiclass logestic regression with 4 outputs [0,0],[0,1],[1,1],[1,1] but I wouldn't get individual probabilities and It felt safe to assume the target variables are independent. 
I got stuck at the part where test data also had null values, using which i could not test the model . So i tried using simple imputer to fill in the values , 
but the columns that needed encoding are different so when i used  one hot encoder the columns are getting different . i couldn't  progress any further from there.
