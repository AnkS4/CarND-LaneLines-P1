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
