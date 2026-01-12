# Trajectory and Road Analysis

This project evaluates and improves the map matching performance in urban environments using the Porto taxi trajectory dataset. 

We first apply Fast Map Matching (FMM) to 1,481 trajectories as the baseline and observe that the original configuration fails on a subset of cases due to GPS noise, sparse sampling, and insufficient candidate-road search range.

To address these issues, we propose a two-layer enhancement strategy: 

(1) Improving the robustness of FMM through parameter tuning—including enlarging the search radius, increasing the number of candidates, and relaxing the GPS error threshold

(2) Employing the spatio-temporally constrained ST-MATCH algorithm as a fallback when necessary. 

Experimental results show that the combined approach increases the overall matching success rate to above 99%, effectively resolving the failure cases in the baseline method. Our findings demonstrate that parameter optimization, together with complementary algorithmic collaboration, is an effective way to enhance the accuracy and robustness of map matching for urban trajectory data.

### Tech Stack Used

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![GeoPandas](https://img.shields.io/badge/GeoPandas-139C5A?style=for-the-badge&logo=python&logoColor=white)
![OSMnx](https://img.shields.io/badge/OSMnx-000000?style=for-the-badge&logo=openstreetmap&logoColor=white)
![Shapely](https://img.shields.io/badge/Shapely-2E7D32?style=for-the-badge&logo=python&logoColor=white)
![FastMapMatch](https://img.shields.io/badge/FastMapMatch-1976D2?style=for-the-badge&logo=python&logoColor=white)



### Tasks

In this project, we perform several tasks of preprocessing, visualizing and query processing of trajectory data. The following tasks (same name as source code file) are highlighted in this repo (as per my contribution towards the project)

#### Task 2

Visualizing the raw GPS points of the first 15 trips in the trajectory data dataset on a map with the road network of Porto.

#### Task 3

Map Matching with Fast Map Matching (FMM)  

The raw GPS points are inaccurate. Some common causes of these inaccuracies include low quality hardware, signal interference and atmospheric conditions. This leads to GPS points being out of place where no road is   present or trajectories not following an actual path.

Hence, to correct this map matching algorithms are used. A map matching algorithm is a technique typically used to align the coordinates (often captured via a GPS) with the road network. This helps in correcting      the positional error and improving the plotting of trajectories.

To further improve the coverage of trips, hyperparameter tuning was performed alongside using ST-Match as a backup matcher (This is not covered in the code, as this is a group project and I am only documenting my     contents)

#### Task 4

Visualizing the map-matched routes that of the first 15 trips.


## Academic Context
Completed during my Graduate studies at **Nanyang Technological University (NTU), Singapore**.

* **Course:** Urban Computing
* **Semester:** AY 2025/2026, Semester 1
* **Grade Achieved:** A


## Usage
**Note for current/future NTU students:** While this repository is public, please ensure you adhere to NTU's Academic Integrity Policy. This is intended as a reference for my personal portfolio; using this code for your own graded assignments is strictly prohibited by the University.
