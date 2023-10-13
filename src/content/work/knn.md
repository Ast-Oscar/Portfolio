---
title: K-nn predictions
publishDate: 2023-01-25 00:00:00
img: ../../assets/knn_miniature.jpg
img_alt: knn algorithm
description: |
  In my third year, I wrote a Python program that could predict the classes of variables of a dataset by training it on another dataset with the k-nn algorithm
tags:
  - Python
  - k-nn mean
---

<h4>The process</h4>
<p style="width: 100%">
  The algorithm behind it is pretty simple:
  
  - We import the dataset.
  - We use it to train our algorithm, it will learn the probabilities of being of one class when your "k" (k is an integer) neighbours are of certain classes.
  - To make sure it works, we train the algorithm on half the dataset and predict the other half.
  - We compare the predictions with the dataset (we make a **confusion matrix**)
  - Once done, we create a loop of this process with different k=1,2,3... To select the best k possible.
  
  We then take the dataset that we have to predict (it was the project of the class) and use our trained algorithm on it. it gives us a result.
</p>
