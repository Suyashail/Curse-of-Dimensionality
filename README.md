# Curse-of-Dimensionality
An attempt to understand the Curse of Dimensionality phenomenon.

This code was developed to understand the problems that are associated with the curse of dimensionality phenomenon and to try out a different approach for the same to get better results.


The curse of dimensionality introduces the following problems:
1. Points in higher dimension space tend to accumulate around the edges of a n-dimensional cube
2. The distance a new point in the n-dimensional space is equidistant to every point in the n-dimensional space (Nearest Neighbour algorithm fails in high dimension).
3. Higher number of training samples required foe efficient training of the machine learning models.


In this sample notebook, we compare the results of sampling points from an n-dimensional cube and an n-dimensional sphere. Sampling of the points from an n-dimensional sphere results in improvements on the first and the second problem. 

This code is still in beta/developmental state (only intended for understanding of concept). Any improvements for the same are encouraged.
