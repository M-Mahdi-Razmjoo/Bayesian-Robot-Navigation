# Bayesian-Robot-Navigation

This repository contains an end-to-end implementation of a Bayesian network-based robot navigation system. The project demonstrates how probabilistic reasoning can guide a robot's movement in an uncertain environment using conditional probability distributions (CPDs), exact inference (via variable elimination), and sampling methods.

## Project Overview

- **Bayesian Network Modeling:**  
  Models key factors (e.g., Weather, Battery Level, Goal Distance, Sensor Accuracy, Obstacle Detection, Move Success, and Robot Position) as nodes in a directed graph. The dependencies among these variables are defined by CPDs.

- **Inference Techniques:**  
  Implements:
  - **Variable Elimination:** For exact inference.
  - **Sampling Methods:** Including Prior Sampling, Likelihood Weighting, and Gibbs Sampling, to approximate the posterior distribution of the robot's position.

- **Robot Navigation:**  
  A `RobotNavigation` class uses the Bayesian inference methods to decide the robot’s next move on a grid. The robot updates its state based on environmental factors and navigates towards a goal while avoiding obstacles.
