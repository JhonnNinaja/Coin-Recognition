
**Description:**

This Python code uses computer vision techniques with OpenCV to detect and count coin values in an image. The process includes the following steps:

1. **Image preprocessing:**

* Reading an input image.
* Converting to grayscale.  
* Applying Gaussian blur to reduce noise and smooth unimportant elements.
* Binarizing the image using an adaptive threshold.
* Eroding the image to remove unwanted elements.

2. **Contour detection:**

* Using Canny function to detect edges.
* Finding the different contours in the image.

3. **Coin identification and counting:** 

* Drawing the contours on the original image.
* Iterating through each contour:
* Calculating contour centroid.
* Calculating contour area.  
* Determining coin denomination based on area.
* Drawing a label with the coin value near its center.

4. **Results:**

* Displaying the processed image with detection and labels. 
* Showing total value of detected coins.

**Dependencies:**

* Python 3
* OpenCV
* Matplotlib
* NumPy

**Installation:** 

1. Install OpenCV, Matplotlib and NumPy using pip:

```bash
pip install opencv-python matplotlib numpy
```

2. Make sure you have the image file (`coins.jpeg`) in the same directory.

