# Image Exposure Classification and Correction

## Project Overview

This project focuses on classifying and correcting the exposure levels of images using MATLAB. 
The dataset includes 101 images categorized into three classes: 
- correctly exposed
- underexposed
- overexposed.
The goal is to automate exposure correction and achieve optimal image brightness.

## Methodology

- **Dataset Creation**: 101 images manually classified into three exposure levels (31 underexposed, 33 overexposed, and 37 correctly exposed).
- **Preprocessing**:
  - Images converted to grayscale and resized to 480 × 640 pixels.
  - Low-level features (mean, variance, skewness, entropy) extracted for classification.
- **Classification**:
  - Models trained using SVM and Decision Tree with K-fold cross-validation (5 folds).
  - Decision Tree achieved the highest accuracy at 90.10%.
- **Correction Process**:
  - Gamma correction applied iteratively to adjust brightness.
  - Decision Tree used to predict corrected image classes.
  - **86%** of corrected images classified as correctly exposed.

## Key Results

- **Model Performance**: Decision Tree outperformed SVM, particularly in handling overexposed images.
- **Correction Insights**: Gamma correction effectively adjusted brightness but highlighted variability across different images.
- **Final Accuracy**: 86% of corrected images classified as correctly exposed.

## Conclusion

This project successfully demonstrated automated exposure classification and correction. 
While effective, finding improved methods for gamma correction could enhance performance.
