# WRT Code Challenge – GSoC 2026

## Overview
This repository contains my work on the Weather Routing Tool (WRT) code challenge.

## Work Done
- Set up and ran WRT
- Generated synthetic weather and depth data
- Ran routing simulations for:
  - Base configuration
  - Coastal routing
  - Optimized routing
  - Minimum time route
- Visualized routes using QGIS

## Unit Test
- Implemented a pytest for `RoutingProblem.get_power`
- Used mocking to isolate dependencies
- Ensured correct fuel calculation behavior

## Data Preparation
- Created synthetic weather dataset using `generate_weather.py`
- Created depth dataset using `create_depth.py`
- This allowed controlled testing of routing behavior

## Observations
- Base and optimized routes were similar
- Coastal routing produced more detailed paths using waypoints
- Genetic Algorithm did not produce outputs in my setup
- This highlights the importance of testing and validation

## Conclusion
This exploration motivated my proposal to improve the testing framework of WRT, especially for validating optimization algorithms and ensuring reproducibility.

## Structure
- `tests/` → unit test
- `configs/` → routing configurations
- `scripts/` → data generation
- `outputs/` → route results