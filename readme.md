### Introduction
This python package implements Spatial Pyramid Matching [1] to recognize images under different categories. Furthermore, Earth Mover's distance [2] is also incorporated to better align parts of images when calculating image-to-image distance. 

For better explanation, please refer to [my report](https://dl.dropboxusercontent.com/u/37572555/Github/Image%20Recognition/ImageRec.pdf).


### Dependencies
1. python 2.7.x
2. sklearn
3. vlfeat (extract SIFT features)
4. numpy
5. scipy


### Usage 
Below are two examples of two approaches to recognise images.
	
	python SpatialPyramidExample.py
	python EarthMoverDistanceExample.py

### Data Set

The image data set, in which there are six classes (shooting, playing guitar, running, phoning, riding bike and riding horse) as shown in Figure 13, comes from [[3]](https://github.com/lipiji/PG_BOW_DEMO). For each class, there are 60 images with different backgrounds, different persons and different viewpoints.

![dataSet](https://dl.dropboxusercontent.com/u/37572555/Github/Image%20Recognition/imageSet.png)

### Performances
Recognition accuracies (percent) of different pyramids using SVMs with different kernels
![result](https://dl.dropboxusercontent.com/u/37572555/Github/Image%20Recognition/result1.png)

Comparison of recognition accuracy (percent) between aligned distance and unaligned distance![result](https://dl.dropboxusercontent.com/u/37572555/Github/Image%20Recognition/result2.png)

### References
[1] S. Lazebnik, C. Schmid, and J. Ponce, “Beyond bags of features: Spatial pyramid matching for recognizing natural scene categories,” in Computer Vision and Pattern Recognition, 2006 IEEE Computer Society Conference on, vol. 2. IEEE, 2006, pp. 2169–2178.

[2] Y. Rubner, C. Tomasi, and L. J. Guibas, “The earth mover’s distance as a metric for image retrieval,” International Journal of Computer Vision, vol. 40, no. 2, pp. 99–121, 2000.

[3] P. Li, J. Ma, and S. Gao, “Actions in still web images: Visualization, detec- tion and retrieval,” in Web-Age Information Management. Springer, 2011, pp. 302–313.


