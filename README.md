# ML-Minor Project-Image-Classification

Image classification has become one of the key pilot use cases for demonstrating machine learning.

Inside a dataset we have two directories-
1. Train: This directory contains the images used for training.
2. Test: This directory contains the images used for testing the training quality.

The dataset used for this model has 3 categories: 'Boots', 'Heels' and 'Sport Shoes'.
This model will help you in identifying an image of a footwear into these categories.

## Steps involved in the model creation:
### 1. Reading and Processing the dataset
First, we read the dataset from the source and then process it by resizing and flattening of the images.
We name the input(features) and target(labels) data as x and y, respectively.

### 2. Splitting into testing and training data
Next, we split our data into a test and training set. 
For this we will use the train_test_split function from scikit-learn. 
We will use 70% of the total set for training and the remaining for the test set.

### 3. Applying Classification Algorithm
Next we apply any classification algorithm with best hyper parameters.
The algorithm used in this model is LogisticRegression from scikit-learn.
(For reference, i also gave the code for K Nearest Neighbors, RandomForestClassifier and Naive Bayes algorithms.)
Important Parameters for deciding the performance of a LogisticRegression Model are 'C' and 'penalty'

### 4. Fitting and Predicting
Next we fit the model and predict values for the test data.
To find the accuracy of the model, we compare the predicted values with actual test data values.

### 5. Evaluation
Now we evaluate the model using Confusion Matrix and Classification Report.

### 6. Saving the model
Since this is the last stage of the model creation so we can now save the model using pickle library.

### 7. Predictiong for a new image(other than daaset)
then using the saved model we can Predict for any new Image as to which category does it belong.

Refer to this Code: https://colab.research.google.com/drive/1ZR3kuvqObJ5v_sY4iTgHkkUVgrce5YPv
