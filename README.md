## Advanced Lane Finding
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)
![Lanes Image](./examples/example_output.jpg)

In this project, the goal is to write a software pipeline to identify the lane boundaries in a video.

The Project
---

The goals / steps of this project are the following:

* Compute the camera calibration matrix and distortion coefficients given a set of chessboard images.
* Apply a distortion correction to raw images.
* Use color transforms, gradients, etc., to create a thresholded binary image.
* Apply a perspective transform to rectify binary image ("birds-eye view").
* Detect lane pixels and fit to find the lane boundary.
* Determine the curvature of the lane and vehicle position with respect to center.
* Warp the detected lane boundaries back onto the original image.
* Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.

**The Pipeline**
---

Removal of camera lens distortion:
![Lanes Image](./output_images/undistorted.png)

Verification of perspective transform matrix:
![Lanes Image](./output_images/perspectiveCheck.png)

Converting image to top-view perspective and thresholding using a combination of Sobel gradients and saturation
![Lanes Image](./output_images/thresh.png)

Curve fitting to obtain lanes and the lane region
![Lanes Image](./output_images/lane_region.png)

Annotation with radius of curvature of lanes and the distance of vehicle from center of lanes:
![Lanes Image](./output_images/result.png)

**Result**
---

[![Lanes Video](./examples/example_output.jpg)](./project_video_output.mp4) "Lane Tracking")
![Lanes Video](./project_video_output.mp4)

**Execution**
---

run tracklanes.ipynb on jupyter notebook
