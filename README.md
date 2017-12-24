# **Finding Lane Lines on the Road** 

## Pipeline Description

To identify the lane lines I did the following steps:

1. Made a copy of the image
1. Converted the image to grayscale.
2. Applied image smoothing to gray image by GaussianBlur.
3. Then, applied Canny Edge detection on blurred image.
4. Identified region of interest.
5. Masked the canny output image in region of interest.
6. Applied Hough Transform to masked image.
7. To make the lines semi-transparent, used addWeighted() function & drawn it over the original image.
8. Modified draw_lines() to extrapolate the line segments.

![Original Image](/images/0.jpg)
![Gray Image](/images/'1 Gray Image.png')
![Blurred Image](/images/'2 Blurred Image.png')
![Canny Image](/images/'3 Canny Image.png')
![Masked Image](/images/'4 Masked Image.png')
![Hough Lines](/images/'5 Hough Lines.png')
![Detected Lanes](/images/'6 Detected Lanes.png')


## Potential Shortcomings

## Possible Improvements
