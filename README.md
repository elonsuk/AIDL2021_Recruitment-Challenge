# AIDL2021_Recruitment-Challenge
Analysis based on Kaggle's "Top Streamers on Twitch 2020" dataset. Predictions for the number of Followers gained are made based on the other features available in the dataset. Analysis is done via mainly utilizing the Tensorflow 2.6 and Keras API, and other regression APIs. Also a recruitment challenge for joining AIDL 2021 at HKUST.

<br>```Final Solution.ipynb```: This file is not used for making prediction results. Although predictions are made, I did not upload this on Kaggle. Still, evaluation of the RMSE results are made internaly in the project. This note deals the ultimate way of approach in an organized manner I discovered through numerous trials and failures made thoughout the challenge. This includes Feature Engineering and the generation and training of a Deep Neural Network model. If you want to read through the most generally implemented solution for this type of regression problem, read this. While, if you want to explore the various attempts and mistakes made during this challenge, read through the other notes in the ```Attempts_Collection``` folder.

<br>**.ipynb files**

<br>```Trial 1_5LDNN.ipynb```: Got a RMSE loss value of 424781.02578, what a shame. Made some mistakes here; I wouldn't go through this again, but this will remain here.
<br>- DNN model consists 5 layers in total - 2 respective input and output layers; 3 hidden layers.

<br>```Trial 2_Data Augmentation+9LDNN.ipynb```: Augmented the dataset by adding random artificial data that lies in the IQR range of Followers gained. Got a RMSE loss value of 101719.34368; significant improvement since the previous trial. Yay.
<br>- DNN model consists 9 layers in total - 2 respective input and output layers; 7 hidden layers.

<br>```Trial 3_Outliers Removed+Data Augmentation+9LDNN+Stacked Model.ipynb```: Augmented the dataset after removing the outliers, used a Deep Neural Network model and a stacked model of XGBRegressor, LGBMRegressor, and Random Forest Regressor for training and making predictions. Got a RMSE loss value of 124260.55540; this rather degraded in performance relative to the model from Trial 2.

<br>**.csv files**

<br>```Trial_4_Predictions.csv```: Predictions from the fourth trial. Trial 4 solely utilized the 9LDNN model from Trial 3 for training and making predictions. Model file got accidentally deleted, but refer to Trial 3 for the details of the DNN model.
