# knn-big-data

The object of this project is to implement the KNN algorithm proposed by [Zhenyun Deng, Xiaoshu Zhu, Debo Cheng, Ming Zong, Shichao Zhang, Efficient kNN classification algorithm for big data, Neurocomputing].

## Algorithm
Algorithm. The pseudo of LC-kNN algorithm.
Input: Training dataset, test samples Y;
Output: Class label;
1 Produce m cluster centers using LSC algorithm, denoted by
C1,C2,C3,......,Cm;
2 Compute the distance D(y,Ci) between test sample y and
each cluster center,denoted by D(y,Ci), i = 1,2,...,m;
3 Compute the nearest cluster center Ci to y, Ci = min{D(y,Ci)},
i = 1,2,...,m;
4 Using the corresponding cluster of Ci as the training dataset,
denoted by NewXi;
5 Apple to kNN algorithm to predict y in the training dataset.


## Datasets
* GISETTE: GISETTE is a handwritten digit recognition problem. The problem is to separate the highly confusible digits '4' and '9'. This dataset is one of five datasets of the NIPS 2003 feature selection challenge. Source: https://archive.ics.uci.edu/, UCI Machine Learning Repository.

* OPTDIGITS: Used preprocessing programs made available by NIST (http://yann.lecun.com/exdb/mnist) to extract normalized bitmaps of handwritten digits from a preprinted form. From a total of 43 people, 30 contributed to the training set and different 13 to the test set. 32x32 bitmaps are divided into nonoverlapping blocks of 4x4 and the number of on pixels are counted in each block. This generates an input matrix of 8x8 where each element is an integer in the range 0..16. This reduces dimensionality and gives invariance to small distortions.
Source: https://archive.ics.uci.edu/, UCI Machine Learning Repository.


## Tech
* Python
* PySpark
* ScikitLearn