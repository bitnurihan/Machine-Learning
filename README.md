# Machine-Learning for TAR
1. Purpose
- Test to change modeling method from scikit learn(curve_fit) to machine learning.

2. Difference with previous modeling
- To maintain user can set cprp(or cpm), 'cost to grp' and 'grp to reach' methods are retained.
- Previously, only grp could be used to calculate reach%, but cost added to x value in this model.
- Previous modeling(by python & R) has been calculated constants and coefficients by target(over 200), so it's spent a lot of time on modeling and testing, but now can see the results of all targets in just two models.

3. Methodology
- Supervised learning through tensorflow.
- Convert 'cost' and 'grp' to log.
- Pre-processing uses robust scalar.
- Categorical variables(targets, channels) are handled by one-hot encoding.
- Among the variables affecting reach%, 'month' is divided into relatively high month (December-February) and another(March-November).
- Outlier detection of raw data uses IQR.
- Because it is nonlinear regression, activation is selected to 'relu'.
- Only one hidden layer is set.

** Raw data can't be uploaded because it's confidential.
