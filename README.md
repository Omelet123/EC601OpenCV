# EC601OpenCV
gyt@bu.edu
This is the exercise for OpenCV. 
###EX1
Q:How does a program read the cvMat object, in particular, what is the order of the pixel structure?
Image is built by pixels. OpenCV read images through every pixel.
For example:
I read the picture Lenna in three ways which are RBG, Gray and RBG with Alph Channel. Then I print them out.
Grayscal is 2-dimensional array and the other two are 3-dimensional array.
The output is:
RGB:
[[[125 137 226]
  [125 137 226]
  [133 137 223]
  ..., 
  [122 148 230]
  [110 130 221]
  [ 90  99 200]]

 [[125 137 226]
  [125 137 226]
  [133 137 223]
  ..., 
  [122 148 230]
  [110 130 221]
  [ 90  99 200]]

 [[125 137 226]
  [125 137 226]
  [133 137 223]
  ..., 
  [122 148 230]
  [110 130 221]
  [ 90  99 200]]

 ..., 
 [[ 60  18  84]
  [ 60  18  84]
  [ 58  27  92]
  ..., 
  [ 84  73 173]
  [ 76  68 172]
  [ 79  62 177]]

 [[ 57  22  82]
  [ 57  22  82]
  [ 62  32  96]
  ..., 
  [ 79  70 179]
  [ 81  71 181]
  [ 81  74 185]]

 [[ 57  22  82]
  [ 57  22  82]
  [ 62  32  96]
  ..., 
  [ 79  70 179]
  [ 81  71 181]
  [ 81  74 185]]]
  Gray:
  [[169 169 168 ..., 175 162 138]
 [169 169 168 ..., 175 162 138]
 [169 169 168 ..., 175 162 138]
 ..., 
 [ 53  53  59 ..., 115 112 114]
 [ 53  53  64 ..., 117 118 122]
 [ 53  53  64 ..., 117 118 122]]
###EX4
Q:What are the disadvantages of binary threshold?
Here, the matter is straight forward. If pixel value is greater than a threshold value, it is assigned one value (may be white), else it is assigned another value (may be black). It can't fit all pictures because it directly split picture into two sets and it will lost a lot of information. It may not be good in all the conditions where image has different lighting conditions in different areas.
Q:When is Adaptive Threshold useful?
Binary threshold used a global value as threshold value so it may not be good in all the conditions where image has different lighting conditions in different areas.In that case, we go for adaptive thresholding. In this, the algorithm calculate the threshold for a small regions of the image. So we get different thresholds for different regions of the same image and it gives us better results for images with varying illumination.
