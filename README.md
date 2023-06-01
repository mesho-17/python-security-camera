# Motion Detection

This Python code detects motion using the webcam and OpenCV library. It captures frames from the webcam and compares them to identify any differences. If significant motion is detected, it draws a rectangle around the moving object and plays a beep sound using the winsound library.

# Prerequisites 

Python 3.x
OpenCV (cv2) library
winsound library (usually comes pre-installed with Python) 

# Installation 

Ensure Python is installed. You can download Python from the official website: Python.org

Install the required libraries using pip:

```shell
pip install opencv-python
```
`pip install winsound`
# Usage

Copy and paste the provided code into a Python file (e.g., motion_detection.py).

Run the Python script:

`python motion_detection.py`

A window will open, showing the live webcam feed.

When motion is detected, a rectangle will be drawn around the moving object, and a beep sound will play.

Press the 'q' key to exit the program.

# Notes

This code uses the first available webcam (index 0). If you have multiple webcams connected, you can change the index to select a different webcam.

The motion detection algorithm compares consecutive frames from the webcam. Adjusting the threshold value (20 in this code) can help filter out noise and detect only significant motion.

The minimum contour area (5000 in this code) determines the size of the moving object that will trigger the motion detection. Adjust this value according to your needs.

The code uses the GaussianBlur function to reduce noise in the grayscale difference image.

By uncommenting the line # cv2.drawContours(frame1, contours, -1, (0, 255, 0), 2), you can draw the contours of the moving objects on the frame.

Ensure that the necessary permissions are granted to access the webcam on your system.
