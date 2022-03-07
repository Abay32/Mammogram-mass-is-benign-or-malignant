
# Predict whether a mammogram mass is benign or malignant
 
This data contains 961 instances of masses detected in mammograms, and contains the following attributes/fields:

BI-RADS assessment: 1 to 5 (ordinal)
Age: patient's age in years (integer)
Shape: mass shape: round=1 oval=2 lobular=3 irregular=4 (nominal)
Margin: mass margin: circumscribed=1 microlobulated=2 obscured=3 ill-defined=4 spiculated=5 (nominal)
Density: mass density high=1 iso=2 low=3 fat-containing=4 (ordinal)
Severity: benign=0 or malignant=1 (binominal)

BI-RADS is an assesment of how confident the severity classification is; 
it is not a "predictive" attribute and so we will discard it. 
The age, shape, margin, and density attributes are the features that we will build our model with, 
and "severity" is the classification we will attempt to predict based on those attributes.

Although "shape" and "margin" are nominal data types, which sklearn typically doesn't deal with well, 
they are close enough to ordinal that we shouldn't just discard them. 
The "shape" for example is ordered increasingly from round to irregular.

A lot of unnecessary anguish and surgery arises from false positives arising from mammogram results. 
If we can build a better way to interpret them through supervised machine learning, it could improve a lot of lives.

# Your Task

Clean the data and normalize it and then apply different supervised machine learning techniques to this data set, 
and see which one yields the highest accuracy as measured with K-Fold cross validation (K=10). Apply:

  - Decision tree
  - Random forest
  - KNN
  - Naive Bayes
  - SVM
  - Logistic Regression
  - Neural network using Keras.
 
Many techniques also have "hyperparameters" that need to be tuned. Once you identify a promising approach, 
see if you can make it even better by tuning its hyperparameters.

# Dependencies 
    - Padas
    - Sklearn 
    - Tensorflow 
    

