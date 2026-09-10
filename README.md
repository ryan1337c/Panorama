# Panorama

Given different images of the same scene, it generates a panorama.

## Overview

This project implements an end-to-end panorama generation system that combines multiple photographs taken from a fixed viewpoint into a single, seamlessly blended panoramic image. The implementation handles feature detection, image alignment, and blending to create high-quality panoramas.

## Features

- **Automatic Feature Detection** - Identifies corresponding points across multiple images
- **Image Registration** - Aligns images using homography transformations
- **Seamless Blending** - Combines images with smooth transitions to avoid visible seams
- **Visualization** - Step-by-step visualization of the panorama generation process

## Project Structure

- **A3.ipynb** - Main Jupyter notebook containing the panorama generation implementation (Part 1 A)
  - Includes complete pipeline from image loading through final panorama output
  - Includes visualizations of intermediate processing steps
  - Demonstrates the core algorithms used for stitching and blending

## Requirements

- Python 3.x
- Jupyter Notebook
- OpenCV (cv2) - for image processing
- NumPy - for numerical operations
- Matplotlib - for visualization

## Usage

1. Open `A3.ipynb` in Jupyter Notebook or JupyterLab
2. Prepare images of the same scene taken from a fixed point with overlapping regions
3. Run the notebook cells to generate your panorama
4. View the visualization outputs to see intermediate results and the final panorama

## How It Works

The panorama generation process typically involves:

1. **Feature Detection** - Detect keypoints in each image using algorithms like SIFT or ORB
2. **Feature Matching** - Match corresponding features across image pairs
3. **Homography Estimation** - Calculate perspective transforms to align images
4. **Image Blending** - Merge images smoothly to create the final panorama
5. **Visualization** - Display results at each stage

## License

MIT License
