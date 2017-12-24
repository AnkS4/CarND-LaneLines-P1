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

(1) Original Image | (2) Gray Image
:-------------------------:|:-------------------------:
<img src="/images/0.jpg" alt="Original Image" width="360"> | <img src="/images/1 Gray Image.png" alt="Gray Image" width="360">

(3) Blurred Image | (4) Canny Image
:-------------------------:|:-------------------------:
<img src="/images/2 Blurred Image.png" alt="Blurred Image" width="360"> | <img src="/images/3 Canny Image.png" alt="Canny Image" width="360">

(5) Masked Image | (6) Hough Lines
:-------------------------:|:-------------------------:
<img src="/images/4 Masked Image.png" alt="Masked Image" width="360"> | <img src="/images/5 Hough Lines.png" alt="Hough Lines" width="360">

(7) Detected Lanes imposed on the Original Image
:-------------------------:
<img src="/images/6 Detected Lanes.png" alt="Detected Lanes" width="360">

## Potential Shortcomings

## Possible Improvements
