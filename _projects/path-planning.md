---
title: 'Highway Path Planning'
subtitle: 'Teaching a car how to navigate around a virtual highway.'
date: 2019-11-16 00:00:00
description:
featured_image: 'images/path-planning/ppcover.png'
---

<p align="center">
  <img width="450" height="350" src="../images/path-planning/ppcover.gif">
</p>

## Overview
* Build a path planner that creates smooth, safe trajectories for the car to follow.
* The simulated highway environment (provided by **Udacity**) has other vehicles, all going different speeds, but approximately obeying the 50 (+- 10) MPH speed limit.
* The subject vehicle transmits its location, along with its sensor fusion data, which estimates the location of all the vehicles on the same side of the road.
* The subject vehicle moves from point to point perfectly, so no controller building is needed. 

### Path planning layers

<p align="center">
  <img width="500" height="450" src="../images/path-planning/overview.png">
</p>

Path planning of an autonomous vehicle is an ensemble of different functional layers.
* **Behaviour** - With the input of previous layers, this layer decides the future state of the subject.
* **Prediction** - This layer identifies entities in a given situation and predicts future changes given sensor perception data.
* **Localization** - It is the layer responsible for understanding the subject's and other entities' current locations.
* **Trajectory** - It calculates the motion flow through space as a function of time.
* **Sensor Fusion** - This layer gathers all the different sensor data helps other layers to make sense of the world.
* **Motion Control** - It's job is to move and control the vehicle.