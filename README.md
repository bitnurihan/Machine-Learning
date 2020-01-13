# Machine-Learning
1. Purpose
- Test to change modeling method from scikit learn(curve_fit) to machine learning.

2. Methodology
- To maintain user can set cprp(or cpm), 'cost to grp' and 'grp to reach' methods are retained.
- Supervised learning through tensorflow.
- Convert 'cost' and 'grp' to log.
- Pre-processing uses robust scalar.
- Categorical variables(targets, channels) are handled by one-hot encoding.
- Among the variables affecting reach%, 'month' is divided into relatively high month (December-February) and another(March-November).
- Outlier detection of raw data uses IQR.
- Because it is nonlinear regression, activation is selected to 'relu'.
- Only one hidden layer is set.
