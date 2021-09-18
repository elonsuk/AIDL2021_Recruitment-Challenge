# AIDL2021_Recruitment-Challenge
Introduction: Analysis based on Kaggle's "Top Streamers on Twitch 2020" dataset. Predictions for the number of Followers gained are made utilizing the Tensorflow 2.6 DNN model. Also a recruitment challenge for joining AIDL 2021 at HKUST.

1. Twitch Data_DNN.ipynb
<br>Main analysis, prediction, and evaluation conducted using the original data. The DNN model has the lowest RMSE loss value, the highest explained variance score and accuracy.

2. Outliers Removed_DNN.ipynb
<br>Forked approach of the main analysis; the identical DNN model and training method is used, while the outliers from the dataset are removed.

3. High Correlation_DNN.ipynb
<br>Forked approach of the main analysis; the identical DNN model and training method is used, while only the columns having a positive correlation with the target prediction value - Followers gained - are used while training and making predictions.

<br>Thanks for reading :D
