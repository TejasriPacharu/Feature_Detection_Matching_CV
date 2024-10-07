# Feature_Detection_Matching_CV
# Image Feature Matching Assignment

## Overview
This project implements image feature matching by detecting key points, describing features using SIFT descriptors, and matching features using Sum of Squared Differences (SSD) and ratio distance. The assignment consists of three main parts:

1. **Keypoint Detection**: Identify points of interest in the image using the Harris corner detection method.  
2. **Feature Description**: Extract Scale Invariant Feature Transform (SIFT) descriptors for each keypoint.
3. **Feature Matching**: Match features between two images using the Sum of Squared Differences (SSD) and ratio distance.

## Table of Contents
- [Keypoint Detection](#keypoint-detection)
- [Feature Description](#feature-description)
- [Feature Matching](#feature-matching)
- [How to Run](#how-to-run)
- [Requirements](#requirements)

## Keypoint Detection
Keypoints in both images are detected using the **Harris corner detection** method, which identifies points of interest based on corner-like regions in the image.

## Feature Description
For each detected keypoint, a **SIFT (Scale Invariant Feature Transform)** descriptor is extracted. SIFT descriptors provide scale and rotation-invariant descriptions of local image regions, making them robust to changes in viewpoint, lighting, and scaling.

## Feature Matching
Features between the two images are matched by comparing the SIFT descriptors using the **Sum of Squared Differences (SSD)**.  
- The **SSD distance** is calculated between each pair of keypoints.
- The **ratio distance** is determined by finding the closest and second closest SSD matches for each keypoint. The ratio is the distance of the closest match divided by the distance of the second closest match.
