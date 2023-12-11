
1.1 data description
	The goal of this project is building and optimizing convolutional network models which can classify  8 different font images accurately. 
The total data set  to be investigated in this project is composed of 8 distinct classes from the subsets from “FONT” dataset. The original data set consists of images from 153-character fonts. Some fonts were scanned from a variety of devices: hand scanners, desktop scanners or cameras. Other fonts were computer generated. In this project, 8 fonts chosen were CANDARA, CONSTANTIA, BORBEL, GRBRIOLA, IMPACT, ITALIC, ROCKWELL, and SYLFAEN. Link of the data set of images is following: https://archive.ics.uci.edu/ml/machine-learning-databases/00417/
Below table[1] is a detailed description of the subsets and the size of the dataset, it shows relatively balanced data instance among 8 font classes.  There are 25136 cases in total.
Font Index	Original Font Name	Font size 	Percentage of Total
1	CANDARA	3024	12.03%
2	CONSTANTIA	3018	12.01%
3	CORBEL	3024	12.03%
4	GABRIOLA	3512	13.97%
5	IMPACT	2716	10.81%
6	ITALIC	3712	14.77%
7	ROCKWELL	2946	11.72%
8	SYLFAEN	3184	12.67%
total		25136	100%
Table[1]: Description of the dataset
Each data instance in a ‘FONT’ file represents an image.  It includes a series of information about a particular image. For example, ‘font’ is the case label; ‘strength’ indicating normal or bold;  ‘italic’: if 1,the image was generated an italic font. ‘originalH’ and  ‘originalW’ represent the height and width of the original image in pixels. Also, it has 400 features describing each of the pixels by grey factor(darkness) 20 x 20 grid which in composite displays each individual character. The maximum value for each pixel is 255 and the minimum value is 0. White is 0, 255 is black. In this project, we focused on 400-pixel value information and used them as our features. 
1.2 data preprocessing
	The 8 data sets were read into Python. X was used to represent 400 features. Thus, the total input feature size is 25136 by 400. For training purposes, input features were reshaped as 25136 by 20 by 20. Also, we normalized the input vectors by dividing each pixel value by 255 so that all the pixel values are in the range of [0,1].Each image has only 1 color channel since it is grey color image. 
To get output of the whole dataset, one hot encoding method was used for every case label. Since there are 8 classes in this dataset, the output size of dataset (represented as Y)is 25136 by 8. 
Train_test_split()function was used to randomly split training set and test set. Test set size is 10% of total data. After splitting, the training set size is 22622, and test set size is 2514. This size of training and test set were equal for 48  models we trained. 
