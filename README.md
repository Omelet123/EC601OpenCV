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
