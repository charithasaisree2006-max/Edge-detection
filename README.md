IMAGE EDGE DETECTION USING SOBEL, PREWITT AND CANNY OPERATORS
![Uploading image.png…]()

# AIM

To demonstrate and compare **image edge detection** using **Sobel, Prewitt, and Canny edge detection operators**.

# SOFTWARE USED

* **Google Colab / VS Code**
* **Python**
* **OpenCV (`cv2`)**
* **NumPy**
* **Matplotlib**

# THEORY

## IMAGE EDGE DETECTION

Image edge detection is a fundamental technique in **image processing and computer vision** used to identify boundaries and significant changes in intensity within an image.

Edges usually represent important features such as object boundaries, shapes, and textures. Edge detection is commonly used as a preprocessing step for tasks such as **image segmentation, object detection, and feature extraction**.

## SOBEL OPERATOR

The **Sobel operator** is a gradient-based edge detection technique used to detect edges in an image.

* It uses two kernels to calculate intensity changes in the **horizontal and vertical directions**.
* The horizontal kernel detects vertical edges.
* The vertical kernel detects horizontal edges.
* The two gradients are combined to obtain the edge strength.

Sobel provides good edge detection while being relatively simple and computationally efficient.

## PREWITT OPERATOR

The **Prewitt operator** is another gradient-based edge detection technique.

* It uses separate kernels for detecting **horizontal and vertical edges**.
* It calculates the intensity difference between neighboring pixels.
* It is simple and computationally efficient.
* It can be used to highlight boundaries and structural features in an image.

## CANNY OPERATOR

The **Canny edge detector** is a multi-stage edge detection algorithm designed to detect clear and thin edges.

The main steps involved are:

* **Gaussian filtering** – reduces noise in the image.
* **Gradient calculation** – identifies changes in intensity.
* **Non-maximum suppression** – produces thin edges.
* **Double thresholding** – identifies strong and weak edges.
* **Edge tracking by hysteresis** – connects relevant edges.

Canny generally produces more refined and well-defined edges compared with simple gradient operators.

## COMPARISON OF OPERATORS

* **Sobel** → Detects horizontal and vertical edges using gradient calculations.
* **Prewitt** → Detects edges using simple horizontal and vertical gradient kernels.
* **Canny** → Uses multiple stages to produce thin and well-defined edges.

The output of each operator may vary depending on the image characteristics and parameter settings.

# CONCLUSION

The experiment demonstrates the use of **Sobel, Prewitt, and Canny operators for image edge detection**. Sobel and Prewitt are simple gradient-based methods for detecting intensity changes, while Canny uses multiple processing stages to produce refined and thin edges. The experiment helps in understanding how different edge detection techniques identify important boundaries and features in an image.
