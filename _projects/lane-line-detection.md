---
title: 'Lane Line Detection'
subtitle: 'A pipeline to identify the lane boundaries in a video from a front-facing camera on a car.'
date: 2019-11-16 00:00:00
description:
featured_image: 'images/lane-finding/car_lanes.jpg'
---

![](/images/lane-finding/lane-finding.gif)

## Overview
The steps of this project are the following:
* Compute the camera calibration matrix and distortion coefficients with a set of chessboard images.
* Apply a distortion correction to raw images.
* Use color transforms, gradients, etc., to create a thresholded binary image.
* Apply a perspective transform to rectify binary image ("birds-eye view").
* Detect lane pixels and fit to find the lane boundary.
* Determine the curvature of the lane and vehicle position with respect to center.
* Warp the detected lane boundaries back onto the original image.
* Output visual display of the lane boundaries and nuemerical estimation of lane curvature and vehicle position.

#### Tech Stack
* Python
* NumPy
* OpenCV

### Camera calibration using chessboard images
A set of chessboard images photographed at different angles were used for this purpose. 
![](/images/lane-finding/1.png&s=400)
<img src="/images/lane-finding/1.png" width="400" height="400">

## See it in Action

<iframe width="1905" height="763" src="https://www.youtube.com/embed/ng9edgddoms" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>