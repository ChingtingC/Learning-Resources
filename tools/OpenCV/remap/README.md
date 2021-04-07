# [remap](https://docs.opencv.org/3.4/da/d54/group__imgproc__transform.html#gab75ef31ce5cdfb5c44b6da5f3b908ea4)

`dst	=	cv.remap(	src, map1, map2, interpolation[, dst[, borderMode[, borderValue]]]	)`

map1: either (x,y) points or just x values having the type CV_16SC2 , CV_32FC1, or CV_32FC2.

map2: y values having the type CV_16UC1, CV_32FC1, or none (empty map if map1 is (x,y) points), respectively.

Note: [convertMaps](https://docs.opencv.org/3.4/da/d54/group__imgproc__transform.html#ga9156732fa8f01be9ebd1a194f2728b7f) for details on converting a floating point representation to fixed-point for speed.

if the shape of src and dst is \[H, W]

* case1:
  * map1 is float32 with shape \[H, W], representing x values.
  * map2 is also float32 with shape \[H, W], representing y values.
* case2:
  * map1 is float32 with shape \[H, W, 2], representing (x, y) values.
  * map2 is `None`.
* case3:
  * map1 is int16 with shape \[H, W, 2], representing the rounding values of (x, y).
  * map2 is `None`.
  * interpolation is `INTER_NEAREST`.
* case4:
  * map1 is int16 with shape \[H, W, 2], representing the floor values of (x, y).
  * map2 is \[u]int16 with shape \[H, W], representing the fraction part of (x, y), \[0 : 4] for the fraction of x and \[5 : 9] for the fraction of y by Q0.5 fixed-point.
  * interpolation is **not** `INTER_NEAREST`.
  * reference: [InterpolationMasks](https://docs.opencv.org/master/da/d54/group__imgproc__transform.html#ga628d8c499433359d67b1d830d46d8dae)
* Not sure(?) cases:
  1. map1 is int16 with shape \[H, W, 2] and map2 is **not** `None` when interpolation is `INTER_NEAREST`.
  2. map1 is int16 with shape \[H, W, 2] and map2 is `None` when interpolation is **not** `INTER_NEAREST`.

