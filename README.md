# Urban-Computing
**1. asf**
**2. Trajectory and Road Network Analysis**

In this project, we perform several tasks of preprocessing, visualizing and query processing of trajectory data.

The following tasks are covered (wrt source code files):
- **Task 2:** Visualizing the raw GPS points of the first 15 trips in the trajectory data dataset on a map with the road network of Porto.
- **Task 3:** Map Matching using FMM

  The raw GPS points are inaccurate. Some common causes of these inaccuracies include low quality hardware, signal interference and atmospheric conditions. This leads to GPS points being out of place where no road is   present or trajectories not following an actual path.

  Hence, to correct this map matching algorithms are used. A map matching algorithm is a technique typically used to align the coordinates (often captured via a GPS) with the road network. This helps in correcting      the positional error and improving the plotting of trajectories.

  To further improve the coverage of trips, hyperparameter tuning was performed alongside using ST-Match as a backup matcher (This is not covered in the code, as this is a group project and I am only documenting my     contents)

- **Task 4:** Visualizing the map-matched routes that of the first 15 trips.
