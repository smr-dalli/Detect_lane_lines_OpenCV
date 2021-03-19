# Lane Lines Detection

[//]: # (Image References)
[image1]: ./img/whiteCarLaneSwitch.jpg "Start"
[image2]: ./img/canny.png "Canny"
[image3]: ./img/segment.png "Segment"
[image4]: ./img/lines.png "Draw Lines"
[image5]: ./img/output.png "Grayscale"
---

## Project Overview

### 1.1 Goal
The goal of this project is to use OPENCV(Computer Vision) and Python to develop an algorithm that can detect and track lane boundaries in a video. The pipeline was designed for the following scenarios:

* Find the Lines in a road for a static Image
* Find the Lines in a road for a video
* Fill in any gaps in the road line markings
* Fill the space between the lines with a colour

### 1.2 Dependencies

* Python 3.x
* NumPy
* Matplotlib (for charting and visualising images)
* OpenCV 



## 2. Pipeline
The  steps invovled in the pipeline are as follows:
![alt text][image1]

### 2.1 Grey & Canny
![alt text][image2]
* Convert Image to Grey
* Using Canny to get the edges of line

### 2.2 Crop
![alt text][image3]
* Crop image with polygon to get just the road in the image

### 2.3 Add Lines
![alt text][image4]
* Get Hough transformation
* Draw Lines filling in gaps by calculating the gradient of lines and averaging
* Fill in gaps between lines

### 2.4 Output
![alt text][image5]




## 3. Potential shortcomings with your current pipeline


.


## 4. Suggest possible improvements to your pipeline

