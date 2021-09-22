# AIDL2021_Recruitment-Challenge
Analysis based on Kaggle's "Top Streamers on Twitch 2020" dataset. Predictions for the number of Followers gained are made utilizing the Tensorflow 2.6 DNN model. Also a recruitment challenge for joining AIDL 2021 at HKUST.

<br>```Trial 1_5LDNN.ipynb```: Got a RMSE loss value of 424781.0, what a shame. Made some mistakes here; I wouldn't go through this again, but this will remain here.
<br>- DNN model consists 5 layers in total - 2 respective input and output layers; 3 hidden layers.

<br>```Trial 2_Data Augmentation+9LDNN.ipynb```: Augmented the dataset by adding random artificial data that lies in the IQR range of Followers gained. Got a RMSE loss value of 101719.3; significant improvement since the previous trial. Yay.
<br>- DNN model consists 9 layers in total - 2 respective input and output layers; 7 hidden layers.

<br>```Trial 3_Outliers Removed+Data Augmentation+9LDNN+Stacked Model.ipynb```: Augmented the dataset after removing the outliers, used a Deep Neural Network model and a stacked model of XGBRegressor, LGBMRegressor, and Random Forest Regressor for training and predictions.
