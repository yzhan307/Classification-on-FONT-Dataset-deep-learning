Datalink:https://archive.ics.uci.edu/ml/machine-learning-databases/00391/
The Data set come from UCI machine learning repository site. In original data,  5 types of hand postures from 12 users were recorded using unlabeled markers attached to fingers of a glove in a motion capture environment. A rigid pattern of markers on the back of the glove was used to establish a local coordinate system for the hand, and 11 other markers were attached to the thumb and fingers of the glove.
 
Source: A. Gardner, J. Kanno, C. A. Duncan, and R. Selmic. 'Measuring distance between unordered sets of different sizes,' in 2014 IEEE Conference on Computer Vision and Pattern Recognition(CVPR), June 2014, pp. 137-143.
The data set can be used for multiple purpose. In the report, for classification purpose, the features of different hand postures were used to recognize different kind of posture types. 
After updating the data set, one of the classes with small amount of  information has been deleted. 
There were 15822 observations in the dataset, observations were classified into 4 classes. Class size was showed in the following table:
Class1	4107
Class2	3556
Class3	3979
Class4	4180
Grand  Count
	15822

	
Features of hand postures were labeled as Xi, Yi, Zi ( 'i' ranges from 0 to 11). The ( x, y, z) was the -coordinate of the i-th unlabeled marker position. Observations has at most 12 markers per record and at least 8markers. Most of the records have 8 markers at average.(from 0 to 7). 
Finally, the report chose the first 8 markers (which includes 24 Features labeled from X0,Y0,Z0,X1,Y1,Z1…….X7,Y7, Z7) as the data features.
