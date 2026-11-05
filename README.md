# Hardware-Efficient Adaptive Multi-Stage X-Ray Image Enhancement Algorithm

## Overview
This project develops an adaptive multi-stage image processing algorithm to improve the visual quality of digital X-ray images. It addresses noise, low contrast, and poorly defined anatomical structures through a combination of denoising, contrast enhancement, and edge-aware sharpening techniques.

## Processing Pipeline

1. **Adaptive Noise Estimation**
   - Laplacian operator
   - Median Absolute Deviation (MAD)
   - Adaptive noise-level classification

2. **Noise Reduction**
   - Adaptive Guided Median Filtering
   - Bilateral Filtering

3. **Contrast Enhancement**
   - Global Histogram Equalization (GHE)
   - Global Contrast-Limited Adaptive Histogram Equalization (G-CLAHE)
   - Adaptive clip-limit selection using SSIM

4. **Image Sharpening**
   - Kriging-Weighted Laplacian Kernels
   - Guided Edge-Aware Smoothing and Sharpening
   - Adaptive sharpening parameter estimation

## Technologies Used
- Python
- OpenCV
- NumPy
- Scikit-image
- Matplotlib

## Performance Evaluation
The algorithm is evaluated using:
- Entropy
- Mean Intensity
- Noise Estimation
- Edge Count and Edge Density
- Average Gradient
- Laplacian Variance (Sharpness)
- Structural Similarity Index (SSIM)
- Mean Squared Error (MSE)

## Key Contributions
- Integrated multi-stage X-ray image enhancement framework.
- Adaptive noise estimation and filtering configuration.
- Combined global and local contrast enhancement.
- Spatially adaptive sharpening using Kriging-weighted Laplacian kernels.
- Quantitative image quality evaluation.
