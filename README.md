# Feature_Scaling
Normalization typically means rescaling the values into a range of [0,1]. 


Standardization typically means rescales data to have a mean of 0 and a standard deviation of 1 (unit variance).

##Feature_Scaling_Normalization_MinMaxScaling_MaxAbsScaling_RobustScaling

the Normalization MinMaxScaling in the ipynd 

Why do we use MIN MAX scaling?

Variables that are measured at different scales do not contribute equally to the model fitting & model learned function and might end up creating a bias. Thus, to deal with this potential problem feature-wise normalization such as MinMax Scaling is usually used prior to model fitting
{from sklearn.preprocessing import MinMaxScaler}



What is standard scaling in machine learning?

Feature Scaling is a technique to standardize the independent features present in the data in a fixed range. It is performed during the data pre-processing to handle highly varying magnitudes or values or units.
{from sklearn.preprocessing import StandardScaler}

What is Mean Normalization?

Mean Normalization is a way to implement Feature Scaling. What Mean normalization does is that it calculates and subtracts the mean for every feature. A common practice is also to divide this value by the range or the standard deviation.


What is Maxabsscaler?

Scale each feature by its maximum absolute value. This estimator scales and translates each feature individually such that the maximal absolute value of each feature in the training set will be 1.0. It does not shift/center the data and thus does not destroy any sparsity.
{from sklearn.preprocessing import MaxAbsScaler}
![mean normalization](https://user-images.githubusercontent.com/68773015/164389788-cf3d0324-6c72-45f6-b274-4d13e3677374.png)



What is a robust scaler used for?

The scale features using statistics that are robust to outliers. This Scaler removes the median and scales the data according to the quantile range (defaults to IQR: Interquartile Range).

Does a robust scaler remove outliers?

By using RobustScaler(), we can remove the outliers and then use either StandardScaler or MinMaxScaler for preprocessing the dataset. It scales features using statistics that are robust to outliers. This method removes the median and scales the data in the range between 1st quartile and 3rd quartile
{from sklearn.preprocessing import RobustScaler}
![robust scaling](https://user-images.githubusercontent.com/68773015/164389878-bb672b11-cf2f-4934-b4b2-f8a5b080820f.png)

