## Bicep Curl Counter - Angle Calculation
This repository provides a Python-based function to calculate the angle between three points in a 2D coordinate system. This can be used to track bicep curls during workouts by monitoring the angles formed by the shoulder, elbow, and wrist.

## Features
Angle Calculation: Computes the angle between three points.

Fitness Tracking: Ideal for analyzing bicep curls or other exercises involving joint movements.

Integration Ready: Can be combined with pose estimation models like Mediapipe or OpenPose for real-time tracking.

## Function Overview
### calculate_angle(a, b, c)

This function calculates the angle between three points and normalizes it between 0° and 180°.

### Parameters:
a: Coordinates [x, y] for the first point (e.g., shoulder).

b: Coordinates [x, y] for the middle point (e.g., elbow).

c: Coordinates [x, y] for the third point (e.g., wrist).

### Returns:
The angle (in degrees) between the three points

## Usage
### Bicep Curl Tracking Example
This function can be used to count bicep curls by monitoring the elbow angle:

Identify the top position of the curl (e.g., angle ≤ 30°).

Identify the bottom position of the curl (e.g., angle ≥ 160°).

Count a repetition each time the angle transitions from bottom to top and back.

## Applications

Fitness Tracking: Use for exercises involving joint movements, like squats, push-ups, or lunges.

Pose Analysis: Integrate with real-time pose detection for movement analysis.

Sports Analytics: Monitor athletic performance or rehab exercises.
