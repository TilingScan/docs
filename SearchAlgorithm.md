# Description of the search algorithm

For the detection of differential expression, the application has been implemented with a search algorithm, that we define as the **"sliding window search algorithm"**. 
Firstly, two main parameters have to selected:

- The first one is the **window size (V)**, that will define the minimum number of probes that will be considered a region of interest. For example, in the case of a data set obtained from a microarray that contains 25mer probes, if regions of 75 or more nucleotides want to be detected, a V=3 will be selected. 
- The second one is the **fold-change threshold (U)**, that will define the minimum fold-change that is required for a region to be considered of significant change. 

Once these two parameters are defined, two adyacent windows of the desired V size (A and B) are defined at the beginning of the data set. 
For each of them, the average intensity value of the probes contained within them is calculated. 
These two windows will slide along the data set, until the difference between the average value of A and the average value of B surpasses the fold-change threshold U. 
When this happens, the start point of a region will be defined from the first point of B. 

To determine the end point of the region of change, a new window (C), of fixed size = V will be created adyancent to the end of B. 
The comparison between B and C will now be repeated in the same way it was done for A and B, this time extending window B until the difference between B and C is equal to the selected threshold (U). 
This will determine the length of the detected region, that will be determined by the start and end point of the extended window B. <br><br>
To prevent false positives from appearing, we establish two criteria that all detected regions muts meet: 

- First, when the start point of a detected region is defined, the average value of window B must be at least a certain percentage value (P) above 0. 
- And second and complementarily to this, if during the extension of window B the average intensity value within it is below (1+U*P) at any time, the end point of the region is then defined. 

All the defined above will serve for the detection of up-regulated regions. 
In order to detect those regions that are down-regulated, the inverse of the signal is calculated, and the same criteria algorithm with the same permutation criteria is applied. 

![](http://tilingscan.uv.es/img/tutorial/13.png)
