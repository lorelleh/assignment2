# AAE5303 Assignment: Visual Odometry with ORB-SLAM3

## Executive Summary

This report presents the implementation and evaluation of **Monocular Visual Odometry (VO)** using the **ORB-SLAM3** framework on the **HKisland_GNSS03** UAV aerial imagery dataset. The project evaluates trajectory accuracy against RTK ground truth using **four parallel, monocular-appropriate metrics** computed with the `evo` toolkit.

### Key Results

| Metric | Value | Description |
|--------|-------|-------------|
| **ATE RMSE** | **2.3346 m** | Global accuracy after Sim(3) alignment |
| **RPE Trans Drift** | **1.6310 m/m** | Translation drift rate (delta=10 m) |
| **RPE Rot Drift** | **106.7148 deg/100m** | Rotation drift rate (delta=10 m) |
| **Completeness** | **80.05%** | Matched poses / total ground-truth poses(1565 / 1955) |
| **Estimated poses** | **2,198** | Trajectory poses in `CameraTrajectory.txt` |

---
