# OpenCV

## installation

`pip install opencv-python`

or

`conda install opencv` for conda

or refer to https://docs.opencv.org/master/da/df6/tutorial_py_table_of_contents_setup.html

## usage

1. import

`import cv2`

2. imread

`img = cv2.imread('image.jpg')`

`img_gray = cv2.imread('image.jpg', cv2.IMREAD_GRAYSCALE)`

  * cv2.IMREAD_COLOR
  * cv2.IMREAD_GRAYSCALE
  * cv2.IMREAD_UNCHANGED

3. imwrite

`cv2.imwrite('output.jpg', img)`

`cv2.imwrite('output.png', img)`

`cv2.imwrite('output.tiff', img)`

`cv2.imwrite('output.jpg', img, [cv2.IMWRITE_JPEG_QUALITY, 90])  # 0 ~ 100`

`cv2.imwrite('output.png', img, [cv2.IMWRITE_PNG_COMPRESSION, 5]) # 0 ~ 9`

4. imshow

```
cv2.imshow('My Image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

ref: https://blog.gtwang.org/programming/opencv-basic-image-read-and-write-tutorial/
