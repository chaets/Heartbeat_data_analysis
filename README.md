# Heartbeat_data_analysis
## Heartbeat_data_analysis after reading ECG data
## Heartbeat Data Analysis
### Tools Used
Scipy, Numpy, Seaborn, Matplotlib, Sklearn, Pandas, 

### Data Import
I have used A00003.mat file for my analysis, it’s a dictionary which have values for heartbeat from ECG. Data is described as 
count	18000
mean	-6.78917
std	149.181
min	-1041
0.25	-36
0.5	20
0.75	57
max	520

![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f1.png)
Figure 1


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f2.png)
Figure 2


 In these graphs we can clearly see the outliers and bad values which be eliminated from the data sets.

## First method: -
Smoothing technique
![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f3.png) 
Figure 3


We can see the graph clearly the green line shows appropriate beat from the data.
So using Zscore and setting up threshold, we removed the outliers as shown in graph 1


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f4.png) 
Figure 4

![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f5.png) 
Figure 5


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f6.png) 
Figure 6


In the graph we can clearly see that values greater than 500 is adjusted. 
Now I have tried another method to clean up the data, using mean and value adjusting us standard deviation.


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f7.png) 
Figure 7


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f8.png) 
Figure 8


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f9.png) 
Figure 9


Now after creating dataset from mean and Standard deviation values, I also applied K means clustering in new dataset.


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f10.png) 
Figure 10


We also checked kmean clustering on original dataset.
![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f11.png) 
Figure 11


Finally, I have checked Nearest neighbor algorithm and Kmean clustering algorithm but it dosesnt provide appropriate solution through it.


![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f12.png) 
Figure 12


Eigen values for checking elbow of the graph
![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f13.png) 
Figure 13


Eigen vector demonstration
![alt text](https://github.com/chaets/Heartbeat_data_analysis/blob/master/f15.png) 
Figure 14

