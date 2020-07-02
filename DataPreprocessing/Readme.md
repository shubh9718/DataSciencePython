"Data" dataset contains a retail company's data to predict whether or not a customer buys the product.

For Feature Scaling we can choose either standardisation or normalisation. Normalisation is more suited for normal distribution of data. Standardisation is suited for any type of data, so I have used standardisation here.
Notes:
1) For standardisation((x-mean(x))/standardDeviation(x)), the value of mean and standard deviation will be used of training set for both training and test set because we want the test set to be treated separately as a new dataset.
2) The splitting of dataset must be performed before feature scaling because we want the test set to be a new dataset different from training dataset. If we apply feature scaling before, the scaled data will also contain some traces of test dataset which we do not want.
3) For feature scaling we won't need the encoded columns because we already have them in range of 0,1. Standardisation outputs values between -3,3. So it will only make the already encoded classes more complex.
4) Fit method of standard_scaler computes mean and standard deviation. Transform method applies the main formula of standardisation. So for train set, we apply fit_transform to do both, and for other sets we only use transform because of 3rd point above.
