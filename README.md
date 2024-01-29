# Air-Canvas_Cv2
Create Air Canvas using Python-OpenCV
 Air Canvas which can draw anything on it by just capturing the motion of a colored marker with a camera. 
Here a colored object at the tip of the finger is used as the marker.
Here Color Detection and tracking are used in order to achieve the objective. The color marker is detected and a mask is produced. 
It includes the further steps of morphological operations on the mask produced which are Erosion and Dilation. 
Erosion reduces the impurities present in the mask and dilation further restores the eroded main mask.

Requirements:
installed
 1.Python3  2. NumPy  3.  OpenCV

Algorithm:

*Start reading the frames and convert the captured frames to HSV color space (Easy for color detection).
*Prepare the canvas frame and put the respective ink buttons on it.
*Adjust the track bar values for finding the mask of the colored marker.
*Preprocess the mask with morphological operations (Eroding and dilation).
*Detect the contours, find the center coordinates of largest contour and keep storing them in the array for successive frames (Arrays for drawing points on canvas).
*Finally draw the points stored in an array on the frames and canvas.
