# cany-edge-detection
Canny Edge Detection is a popular edge detection technique used in image processing and computer vision to identify the boundaries or edges of objects within an image. It was developed by John F. Canny in 1986. The method is widely used because it can detect edges accurately while reducing noise and avoiding unnecessary edges.

# Features
1. Noise Reduction – Reduces image noise before detecting edges.
2. Accurate Edges – Detects object boundaries clearly and precisely.
3. Thin Edges – Produces thin and well-defined edges.

# Technologies Used
1. Python – Used to implement the Canny Edge Detection algorithm.
2. OpenCV – Provides the Canny() function for edge detection.
3. MATLAB – Can be used for image processing and Canny edge detection.

# How to Use
1. Convert to Grayscale – Convert the input image into a grayscale image.
2. Apply Canny Algorithm – Set low and high threshold values to detect edges.
3. Display the Output – View the resulting image containing the detected edges.

# Applications
1. Medical Imaging – Detects boundaries of organs and abnormalities.
2. Autonomous Vehicles – Helps detect lanes, roads, and obstacles.
3. Object Detection – Identifies object shapes and boundaries in images.

# Program
~~~
DEVELOPED BY
NAME: SUDHARSHINI.G
REGISTER NO: 212225220106

import cv2
import matplotlib.pyplot as plt
img = cv2.imread('photo sudharshini.jpeg',cv2.IMREAD_GRAYSCALE)
blurred =cv2.GaussianBlur(img, (5,5),0)
edges = cv2.Canny(blurred, 50, 150)
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()

~~~
# output
<img width="886" height="540" alt="image" src="https://github.com/user-attachments/assets/7fb90c8a-df86-40df-b316-5d4d68c4a97e" />



