# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./test_images_output/output_image_2.jpg "one of the results"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I used canny edge detection.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by using ransac regression which like a liner regression.

If you'd like to include images to show how the pipeline works, here is how to include an image: 

[image1]: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when car runs on curving road.
This is because I use liner regression as a draw line function. It works well only under premise that road is straight.

Another shortcoming could be what would happen when lane line's color and road's color are almost same.



### 3. Suggest possible improvements to your pipeline

A possible improvement would be to introduce gradient threshold for draw line function.
This will work when my finding lane line detect non-lane object as lane and 

Another potential improvement could be to use curve fitting.


