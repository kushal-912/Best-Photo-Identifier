# Eye Detection using OpenCV and DeepFace

This repository contains Python code for detecting eyes in an image using OpenCV's Haar cascades and DeepFace.

## Prerequisites

Before you begin, ensure you have met the following requirements:

You have installed the latest version of Python.
You have a Windows/Linux/Mac machine with a working internet connection.
You have installed the OpenCV, DeepFace libraries in Python. If not, install with:

Using Eye Detection
To use Eye Detection, follow these steps:

Clone this repository.
Open the Python file in your preferred IDE or text editor.
Replace "your_image.jpg" with the path to your image in the Python file.
Run the Python file.
The code performs the following steps:

Eye detection: The Haar cascade file for eye detection, provided by OpenCV, is loaded. The detectMultiScale function of the eye cascade is used to detect eyes in the image. For each detected eye, a rectangle is drawn around it using the rectangle function of OpenCV.
Pose detection: The code uses MediaPipe’s pose estimation model to detect human poses in the image. If a pose is detected, the score is increased.
Blur detection: The code calculates the variance of the Laplacian of the image to measure the amount of blur. If the image is not blurry, the score is increased.
Brightness score: The code calculates the mean intensity of the image to measure its brightness. If the brightness is within a certain range, the score is increased.
Contrast score: The code calculates the standard deviation of the intensities of the image to measure its contrast. If the contrast is within a certain range, the score is increased.
Contributing to Eye Detection
To contribute to Eye Detection, follow these steps:

Fork this repository.
Create a branch: git checkout -b <branch_name>.
Make your changes and commit them: git commit -m '<commit_message>'
Push to the original branch: git push origin <project_name>/<location>
Create the pull request.
