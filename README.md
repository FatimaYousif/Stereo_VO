# Stereo Visual Odometry

This repository contains the implementation of Stereo Visual Odometry (VO) pipeline in Python on the KITTI dataset. It processes stereo image data to estimate the motion of a camera (w.r.t its starting position) in 3D space. 

## Features
- **Feature detection** using SIFT (Scale-Invariant Feature Transform)
- **Feature matching** using BFMatcher (Brute-Force Matcher)
- **Triangulation** of points
- **3D-2D motion estimation** using PnP (Perspective-n-Point) with RANSAC (Random Sample Consensus)
  
## Requirements
- Python 3.8 or higher
- Required Python libraries:
  - `numpy`
  - `opencv-python`
  - `pytorch`

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/FatimaYousif-01/Stereo_VO.git
2. Navigate to the cloned directory:
   ```bash
    cd Stereo_VO
3. Run the main script:
   ```bash
    python stereo_vo.py
4. For checking the evaluation script:
   - Copy the groundtruth trajectories (_gt.txt) for 10 sequences and their estimated trajectories (_est.txt) in folder  `evo_eval/results`
   - In the eval folder run:
   ```bash
    python evo_metrics.py

## Results
