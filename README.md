#**Finding Lane Lines on the Road**
![Finding Lanes Demo](demo.gif)

Overview
---

When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

In this project you will detect lane lines in images using Python and OpenCV.  OpenCV means "Open-Source Computer Vision", which is a package that has many useful tools for analyzing images.  

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

### Reflection

### 1. Pipeline:
		a. Convert the image into grey scale image.
		b. Perform Gaussian smoothing to reduce image noise.
		c. Perform Canny edge detector to detect edge pixels.
		d. Select the region of interest (ROI) using masking operation.
		e. Further Hough Transform is performed on edge pixels in region of interest.
		f. Subsequently, an image with  lines connecting the edge pixels in ROI is obtained
           which is superimposed over the original image.

### 2. Identify potential shortcomings with your current pipeline
		a. Performance not up to the mark under varied lighting conditions
		b. Static detection of ROI

### 3. Suggest possible improvements to your pipeline
		a. Using region detector operators to get better region of interest.