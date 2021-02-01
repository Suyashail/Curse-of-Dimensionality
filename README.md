# Curse-of-Dimensionality
An attempt to understand the Curse of Dimensionality phenomenon.

This code was developed to understand the problems that are associated with the curse of dimensionality phenomenon and to try out a different approach for the same to get better results.


The curse of dimensionality introduces the following problems:
1. Points in higher dimension space tend to accumulate around the edges of a n-dimensional cube
2. The distance a new point in the n-dimensional space is equidistant to every point in the n-dimensional space (Nearest Neighbour algorithm fails in high dimension).
3. Higher number of training samples required foe efficient training of the machine learning models.


In this sample notebook, we compare the results of sampling points from an n-dimensional cube and an n-dimensional sphere. Sampling of the points from an n-dimensional sphere results in improvements on the first and the second problem. 

This code is still in beta/developmental state (only intended for understanding of concept). Any improvements for the same are encouraged.

Results:
1. Sampling in Cartesian coordinates(1000 points, each of size 1000):
* Number of points on surface of n-D cube: 100
* Mean distance: 13.051196364812087
* Variance: 0.044008756500694884

2. Sampling in Polar coordinates(1000 points, each of size 1000):
* Number of points on surface of n-D sphere: 10
* Mean distance: 1.0778633659601369
* Variance: 0.14210096471024558

Conclusion:
As we can see from the results, when we sample the points in the polar coordiantes, the number of points ending up on the edge reduces drastically (from 100 to 10). This is due to the fact that out of the 1000 dimensions only the first dimension (radius) contributes to the position of the point whereas in cartesian coordinates, even if a single dimension out of 1000 ends up being 1, the point will end up on the edge of the cube. Another interesting point to note is that the variance among the distance between the points in polar coordinates is almost 3 times the variance of distance of points in the cartesian coordinates.
One important thing to note is that the sample size of 1000 points of 1000 dimensions is still very small to make any concrete conclusions about the effectiveness of this method and hence is only presented as a educative material.
