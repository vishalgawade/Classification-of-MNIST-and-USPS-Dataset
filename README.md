#### The classification task will be to recognizing a 28×28 gray scale handwritten digit image and identify it as a digit among 0, 1, 2, ..., 9. We will train the following four classifiers using MNIST digit images.
---
1. Multilayer perceptron neural network classifier.
2. Random Forest classifier.
3. SVM classifier.
4. Logistic regression, which we implement using backpropagation.<br>
5. Combining all models (Ensemble Classifier)
After our four models are trained on MNIST dataset, our task is to use these models to predict output of MNIST testing set which is of 10000 images and on 20,000 images of USPS dataset. We are going to use confusion matrix for evaluation of our models. And finally, we are going to combine the results of all four model’s prediction and apply majority voting using ensemble and predict the final results. Then we will compare results of predicted output and actual target values using confusion matrix and observe how combined model predictions compare to individual model predictions. I am using confusion matrix to calculate the accuracy. Also, we will see does “No Free Lunch” theorem applies to our models and problem in hand.
Out of total 70,000 image samples of MNIST we are going to use 60,000 for training models and 10,000 for testing the model. We are saving the predicted values in csv file so that I can use them later. Let’s see all four models one by one.
