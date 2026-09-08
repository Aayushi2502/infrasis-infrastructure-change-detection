# infrasis-infrastructure-change-detection

This repository contains project documentation and approved visual results only. The source code, datasets, trained models, and implementation details are not included due to confidentiality obligations.

## Overview
INFRASIS is an AI-powered infrastructure monitoring project that detects urban changes from multi-temporal Sentinel-2 satellite imagery. The goal was to identify newly developed infrastructure through pixel-level change detection while reducing false detections caused by clouds, vegetation, and seasonal variation.

Rather than classifying an entire image, the system predicts a change mask for every pixel, making it suitable for large-scale geospatial monitoring.

## My Contribution
- Developed Python-based preprocessing workflows for Sentinel-2 imagery.
- Prepared and processed 200+ Areas of Interest (AOIs) across multiple Indian cities.
- Trained and evaluated a U-Net++ segmentation model for pixel-level infrastructure change detection.
- Built image preprocessing and model inference workflows using PyTorch and OpenCV.

## Technical Approach
1. Collect multi-temporal Sentinel-2 satellite imagery
2. Apply cloud, vegetation, and water masking
3. Align and normalize before/after images
4. Train a U-Net++ segmentation model
5. Generate pixel-level change masks
6. Validate results and reduce false positives

## Example Result

<img width="1280" height="300" alt="image" src="https://github.com/user-attachments/assets/87c36b85-4737-42ce-a6a3-f3ac4afb9c3c" />

## Tech Stack
- Languages: Python
- Frameworks: PyTorch, OpenCV
- Geospatial Tools: Rasterio, GDAL, Sentinel-2
- Model: U-Net++ (Semantic Segmentation)

## Challenges & Learnings
The biggest challenge wasn't training the model—it was improving the quality of the input data. Small image misalignments, cloud cover, and vegetation changes often appeared as false infrastructure changes. Careful preprocessing and data preparation significantly improved the reliability of the final predictions.

> Code and datasets are intentionally excluded in accordance with the project's confidentiality agreement.
