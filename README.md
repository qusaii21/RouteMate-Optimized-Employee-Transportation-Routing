# RouteMate-Optimized-Employee-Transportation-Routing

RouteMate is an advanced bus routing optimization system designed to improve employee transportation by minimizing travel distances between a company depot and employee pick-up points. It leverages clustering and optimization algorithms combined with real-world driving data to create efficient routes for employee transportation.

## Objectives

- **Cluster employees** based on their locations.
- **Optimize bus routes** to minimize total travel distance.
- **Visualize optimized routes** on Google Maps.

## Features

- **Clustering Algorithms**:
  - Utilizes K-Means to group employees based on geographical proximity.
  - Enhances clusters using TLBO (Teaching-Learning-Based Optimization) to refine centroid positions.
- **Real-World Distance Calculations**:
  - Integrates Google Maps Distance Matrix API to compute accurate driving distances.
- **Route Optimization Techniques**:
  - Generates initial routes using the Minimum Spanning Tree (MST) algorithm.
  - Refines routes using the 2-opt algorithm for improved efficiency.
- **Route Visualization**:
  - Generates Google Maps URLs to visualize optimized routes.

## Workflow

1. **Load Data**: Employee locations (latitude and longitude) are loaded from an Excel file.
2. **Clustering**:
   - Employees are grouped into clusters of up to 30, corresponding to bus capacity.
3. **Route Optimization**:
   - Compute driving distances using the Google Maps API.
   - Generate an initial route with MST.
   - Refine the route using the 2-opt algorithm.
4. **Generate URLs**: Create Google Maps URLs for visualizing routes.
5. **Output**: Optimized routes and visualizations for each cluster.

