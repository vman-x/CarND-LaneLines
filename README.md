# **Finding Lane Lines on the Road** 


The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


### Reflection

### 1. My Pipeline

There are mutilple steps involved in my pipeline. In order :
1. Grayscaling the image
2. Applying Gaussian blur to smooth the image
3. Using Canny edge detection to detect the edges
4. Masking the pixels outside ROI
5. Hough Transformation to detect the line segments from edges
6. Extrapolating the lane lines using polyfit and running average


### 2. Potential Shortcoming

Pipeline is specifically designed for lanes with clear lane markings and good sun light. If there are any frames with drastic change in the lighting conditions or the lane markings not clearly visible, then system tend to underperform in such cases.


### 3. Suggest possible improvements to your pipeline

Issue due to varying sunlight can be solved by implementing HSL/HSV filter at the beginning of the pipeline. It should be noted, the system fails in poor lighting conditions.

It can only be used in plains, needs to be tuned for the hilly roads. We can improve the curved line detection using deep learning and neural networks
<br>
> Best regards, 
> Vman

