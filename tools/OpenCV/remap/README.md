# [remap](https://docs.opencv.org/3.4/da/d54/group__imgproc__transform.html#gab75ef31ce5cdfb5c44b6da5f3b908ea4)

`dst	=	cv.remap(	src, map1, map2, interpolation[, dst[, borderMode[, borderValue]]]	)`

map1: either (x,y) points or just x values having the type CV_16SC2 , CV_32FC1, or CV_32FC2.

map2: y values having the type CV_16UC1, CV_32FC1, or none (empty map if map1 is (x,y) points), respectively.

Note: [convertMaps](https://docs.opencv.org/3.4/da/d54/group__imgproc__transform.html#ga9156732fa8f01be9ebd1a194f2728b7f) for details on converting a floating point representation to fixed-point for speed.
