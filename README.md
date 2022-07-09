# Spaceship_Titanic_Kaggle
My model for the famous Kaggle Competition - Spaceship Titanic.


My model's accuracy is **78.6%** with the Leaderboard Top score standing at 85.27%.

Process:
1. Cleaning Data ("train.csv") : Filling nan cells with mean values and selecting only 'k' best features (followed in next point).
2. I imported SelectKBest function from sklearn library to find the "importance" of each feature and then used the best features to create a training set.
3. I then used Keras to create a small Neural Network (3 layers and 2 dropouts = 0.5) and iterated on epochs = 100.
4. I then took the same features from test data("test.csv") to generate a test set and finally inputted it in **model.predict()**.
5. The output values **>= 0.5** were taken as **True** and **others False** and the prediction converted to a .csv file "submission.csv".

If you have any suggestions for improvement of the model (because there is a lot of room for improvement :sweat_smile:), please let me know.   
