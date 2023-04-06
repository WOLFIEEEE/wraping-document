# Document Detection and Perspective Transformation using OpenCV in Python

This Python script captures video from the default camera, applies image processing techniques to extract a document, and then performs a perspective transform to get a bird's eye view of the document. The script is designed to detect documents in a wide range of lighting and backgrounds. The processed document is displayed on the screen in real-time.

## Dependencies:
- cv2
- numpy

## Functions:
- `preProcessing(img)`: Converts the input image to grayscale, applies Gaussian blur, detects edges using Canny algorithm, dilates edges, and erodes the dilated edges.
- `getContours(img)`: Finds and returns the largest contour in the input image.
- `reorder(myPoints)`: Sorts the vertices of the largest contour in a specific order.
- `getWarp(img, biggest)`: Applies a perspective transform to the input image to get a bird's eye view of the detected document.
- `stackImages(scale, imgArray)`: Stacks multiple images horizontally or vertically.

## Usage:
Simply run the main.py file, and the camera will open. Hold up a document in front of the camera, and the script will extract it and display it on the screen. Press "q" to exit the program.
