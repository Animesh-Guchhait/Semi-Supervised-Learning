# Semi-Supervised-Learning

Procedure of this assignment:

1) We read fashion_mnist dataset from keras.

2) Coding has done on four ways:

Fitting Logistic Regression on entire Dataset
Fitting Logistic Regression on randomly selected some datapoints.
Fitting Logistic Regression on selected datapoints(selected datapoints are centroid of k-means).
Fitting Logistic Regression on 20 percentile of closest data selected with respect to centroid.

Observation:

1)Fitting Logistic Regression on entire Dataset accuracy is nearly 84%

2)Fitting Logistic Regression on randomly selected datapoints accuracy is getting reduced gradually.

3)Fitting Logistic Regression on selected datapoints(selected datapoints are centroid of k-means) accuracy is still low but much better than randomly selected datapoints.

4)Fitting Logistic Regression on 20 percentile of closest data selected with respect to centroid . Here accuracy is closest to above process(3) though most of the cases process 3 is better than 4. But result shows process 4 is better than process 2.

Here we iterate the k-value(number of clusters) from 10 to 35 and we observe that for k=18,20,21,22 (k_mean with only centroid) we get better accuracy and reduce error rate (compared to randomly selected datapoints). So, if we have to do semi-supervised learning with k-mean, then value of k between 20 to 22 is prefereble.
