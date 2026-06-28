## Visual Odometry using ORB and OpenCV

This project implements a monocular Visual Odometry pipeline using Python and OpenCV. ORB features are detected and matched between consecutive frames using a 
FLANN-based matcher. The camera motion is estimated by computing the Essential Matrix, recovering the relative rotation and translation, and accumulating the 
transformations over time. The estimated trajectory is then compared with the ground truth trajectory from the KITTI dataset.

**Technologies:** Python, OpenCV, NumPy, KITTI Dataset

**Main steps:**

* ORB feature detection and description
* Feature matching using FLANN
* Lowe's ratio test for outlier rejection
* Essential Matrix estimation
* Camera pose recovery (R, t)
* 3D point triangulation
* Trajectory reconstruction and visualization
