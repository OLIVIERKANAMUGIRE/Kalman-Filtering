# 1D Kalman Filter Example

This repository contains a **simple Python implementation of a 1‑dimensional Kalman Filter** used to track the position of a moving object over time.

The code demonstrates how noisy measurements can be filtered to estimate the true motion of an object using basic linear state‑space models.

## Files

* `kalman_filter.py` (or similar):

  * Implements a `KalmanFilter` class
  * Simulates a 1D moving object
  * Applies prediction and update steps
  * Plots the results

## Description

The Kalman Filter estimates the **position and velocity** of an object assuming constant acceleration. At each time step:

1. The **prediction step** estimates the next state using the motion model.
2. The **update step** corrects the estimate using noisy measurements.

The filter is evaluated by comparing:

* Noisy measurements
* True (simulated) trajectory
* Kalman filter predictions

## Model Assumptions

* State vector: position and velocity
* Constant acceleration input
* Gaussian noise for:

  * Process (acceleration)
  * Measurement (position)

## Output

The script produces a plot showing:

* **Measurements** (blue)
* **Real track** (yellow)
* **Kalman filter prediction** (red)

### Example Result

![Kalman Filter Output](figure.png)

> *Note:* Replace `figure.png` with the actual image file name stored in the repository.

## Requirements

* Python 3
* NumPy
* Matplotlib


## Purpose

This example is intended for **educational purposes**, illustrating the core concepts of Kalman filtering in a clear and minimal way.

---
