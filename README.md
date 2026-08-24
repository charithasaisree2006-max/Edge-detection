IMAGE EDGE DETECTION USING SOBEL, PREWITT AND CANNY OPERATORS
AIM

To demonstrate and compare the effect of Sobel, Prewitt, and Canny edge detection techniques on a grayscale image.

SOFTWARE USED
Google Colab
Python
OpenCV (cv2)
NumPy (numpy)
Matplotlib (matplotlib.pyplot)
THEORY
EDGE DETECTION

Edge detection is an image-processing technique used to identify boundaries and sharp changes in intensity within an image. It is commonly used to detect the shape, structure, and important features of objects in an image.

SOBEL OPERATOR

The Sobel operator detects edges by calculating the intensity gradient in the horizontal (X) and vertical (Y) directions.

The Sobel X and Y gradients are calculated using 3 × 3 kernels. These gradients are then combined to obtain the overall edge magnitude.

Sobel edge detection is simple and provides good results while reducing the effect of noise to some extent.

PREWITT OPERATOR

The Prewitt operator is used to detect horizontal and vertical edges in an image. It uses two 3 × 3 kernels to calculate the intensity gradients in the X and Y directions.

The resulting gradients are combined to identify the edges present in the image.

Prewitt is computationally simple and is useful for detecting basic edges and boundaries.

CANNY EDGE DETECTION

Canny is a multi-stage edge detection technique used to produce thin and well-defined edges.

The main steps involved in Canny edge detection are:

Noise reduction using smoothing.
Calculation of image gradients.
Non-maximum suppression.
Double thresholding.
Edge tracking by hysteresis.

In the program, threshold values of 100 and 200 are used for detecting the edges.

COMPARISON OF EDGE DETECTION METHODS
Operator	Description
Sobel	Detects edges using horizontal and vertical gradients and is simple to implement.
Prewitt	Uses predefined kernels to detect horizontal and vertical edges.
Canny	Produces thinner, cleaner, and better-connected edges compared to Sobel and Prewitt.
CONCLUSION

The experiment demonstrates the application of Sobel, Prewitt, and Canny edge detection techniques on a grayscale image. Sobel and Prewitt are simple gradient-based methods for detecting edges, while Canny provides more accurate and well-defined edges.

Among the three methods, Canny generally produces clearer and thinner edges, making it suitable for applications where precise edge detection is required.
