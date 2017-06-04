# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

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
