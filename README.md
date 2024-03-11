# Deep-learning-challenge
Overview:

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, I’ll use the
features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

Data Preprocessing: 

To begin the data processing we removed any irrelevant information. After dropping EIN and NAME the remaining columns were to be considered features for the model. Name was added back into the second test for binning purposes. The data was then split for training and testing sets. The target variable for the model was labeled “IS_SUCCESSFUL” and has the value of 1
for yes and 0 for no. APPLICATION data was analyzed and “CLASSIFICATION value was used for binning. We used several data points as a cutoff to bin “rare” variables together with the new value of “Other” for each unique value. Categorical variables were encoded by get_dummies() after checking to see if the binning was successful.

 Compiling, Training, and Evaluating the Model:

 There were two layers total for each model after applying Neural Networks. The number of hidden nodes were dictated by the number of features.
 5981 parameters were created by a two-layer training model. The first attempt was just over 72% accuracy which was under a desired 75%.

 Optimization:

 To achevie the target accuracy the following steps were taken under 3 attempts of optimization.
       1. - Dropping more or fewer columns. (Removing 'USE_CASE' column)
          - Creating more bins for rare occurrences in columns.(Change the     threshold for 'Application_TYPE' &'CLASSIFICATION' columns)
        2. - Add more neurons to a hidden layer.(Add more nuurons for both     layers)
           - Add more hidden layers.

        3. - Use different activation functions for the hidden layers.
           - Add or reduce the number of epochs to the training regimen.

Analysis: 

     After attempting several optimization techniques the target accuracy not predicted. Not far from 75%, I will trty  different optimization techniques or model to predict the accuracy.
