# Digit-Classification-Random-Forest
In this project, we were supposed to classify a dataset made of 5 domains with classes of numbers 0 to 9 using random forest classification. In the given dataset for each image we have a specified feature vector and two labels. One of the labels indicates the content of the image (from 0 to 9) and the other is related to the domain label (0 to 4). In the given training data, the specified feature vectors with dimensions of 1024 are taken from 50000 images, 50% used for training and 50% will be used for testing.

# Step 1:
Firstly, used a random forest classification algorithm that works well on the data digit labels, we tuned hyperparameters to achieve the desired accuracy (which we did.). Additionally, in each step, we tested the effect of changing different parameters of the algorithm and calculated the confusion matrix.

# Step 2:
In this step we used a random forest classification algorithm for seperating data by domains and then for each domain, we trained another random forest classification algorithm for digit classification and evaluated the accuracy of the algorithm.

# Step 3:
Eventually, due to missclisification of data, we added data from other domains to domain with high error before classification’s training process, and we got a better result. For this, first, we plotted the confusion matrix of domain classifier and according to the predictions made by the classifier, we decided which digit classifier(s) would increase its accuracy by adding data from another domain to the training data. At the end it was evident that using domain knowledge and adding other domains' data helped us improve the accuracy of the result.
