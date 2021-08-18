# Handling-Imbalanced-Dataset-Feature-Engineering

* In real world, its not uncommon to come across unbalanced data sets where, you might have class A with 90 observations
and class B with 10 observations. One of the rules in machine learning is, its important to balance out the data set or
at least get it close to balance it. The main reason for this is to give equal priority to each class in laymen terms.

<hr>
#### Problem with Imbalanced data 

Feeding imbalanced data to your classifier can make it biased in favor of the majority class, simply because it did not have enough data to learn about the minority.

Let us understand the technique used for creating balanced data sets.

#### Oversampling

This technique is used to modify the unequal data classes to create balanced data sets. When the quantity of data is insufficient, the oversampling method tries to balance by increment the size of rare samples.

A primary technique used in oversampling is SMOTE (Synthetic Minority Over-sampling Technique). In this technique, the minority class is over-sampled by producing synthetic examples rather than by over-sampling with replacement and for each minority class observation, it calculates the k nearest neighbours (k-NN). By doing the we have an advantage of No loss of information and also mitigate over fitting caused by oversampling.

#### Under sampling

Unlike oversampling, this technique balances the imbalance data set by reducing the size of the class which is in abundance. There are various methods for classification problems such as Cluster Centroids and Tomek Links. The cluster centroid methods replace the cluster of samples by the cluster centroid of a K-means algorithm and the Tomek link method removes unwanted overlap between classes until all minimally distanced nearest neighbours are of the same class.By doing the we have an advantage like Run-time can be improved by decreasing the amount of training data set and also helps in solving the memory problems

Balancing the imbalance data is very important in ML in order to achieve the right accuracy . It is not 99% accuracy of the model that matter but the right accuracy of the model matters.There are many more technique used to balanced the imbalanced data . But SMOTE is the one of the common technique used .
