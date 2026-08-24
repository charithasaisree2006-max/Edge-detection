# Edge-detection
Aim
To implement and compare Sobel, Prewitt, and Canny edge detection techniques on a grayscale image using Python and OpenCV, and to visualize the detected edges alongside the original image.

Software Used
Python 3
Google Colab / Jupyter Notebook
OpenCV (cv2) – for image processing and edge detection
NumPy (numpy) – for numerical operations and defining Prewitt kernels
Matplotlib (matplotlib.pyplot) – for displaying and comparing images
Google Drive – for accessing the input image
Theory
Edge detection is an image-processing technique used to identify sharp changes in intensity or brightness in an image. Edges generally represent boundaries of objects, shapes, and important features.

1. Sobel Edge Detection
The Sobel operator detects edges by calculating the intensity gradient in the horizontal (X) and vertical (Y) directions.

In the program:

sobelX = cv2.Sobel(img, cv2.CV_64F, 1, 0, ksize=3)
sobelY = cv2.Sobel(img, cv2.CV_64F, 0, 1, ksize=3)

The X and Y gradients are combined using the magnitude:

G
=
G
x
2
+
G
y
2

Sobel provides good edge detection while reducing the effect of noise to some extent.

2. Prewitt Edge Detection
The Prewitt operator uses two 
3
×
3
 convolution kernels to detect horizontal and vertical edges.

The kernels used are:

K
x
=
[
1
1
1
0
0
0
−
1
−
1
−
1
]

K
y
=
[
1
0
−
1
1
0
−
1
1
0
−
1
]

These kernels are applied to the image using cv2.filter2D(). The resulting gradients are then combined to obtain the detected edges.

3. Canny Edge Detection
The Canny edge detector is a multi-stage edge detection technique. It generally involves:

Noise reduction using Gaussian filtering.
Calculation of image gradients.
Non-maximum suppression to obtain thin edges.
Double thresholding to identify strong and weak edges.
Edge tracking by hysteresis.
In the program:

canny_edges = cv2.Canny(img, 100, 200)

The values 100 and 200 are the lower and upper threshold values used by the Canny detector.

Comparison
Sobel detects edges using horizontal and vertical gradients and is relatively simple.
Prewitt also uses gradient kernels and is computationally simple.
Canny is more sophisticated and generally produces thinner, cleaner, and better-connected edges.
Conclusion
The program successfully applies Sobel, Prewitt, and Canny edge detection to the given grayscale bird image. The three methods demonstrate how different edge-detection operators identify boundaries and intensity changes. Among them, Canny generally provides the clearest and most well-defined edges, while Sobel and Prewitt are simpler gradient-based methods suitable for basic edge detection.



