# PRODIGY_ML_03
# 🐱🐶 Cat vs Dog Image Classification using SVM
This project demonstrates a simple **image classification pipeline** for distinguishing cats and dogs using **Support Vector Machines (SVM)**. The images are loaded directly from a ZIP file, preprocessed, and visualized using **PCA** and sample plots.

## Features

- Load images directly from a ZIP file without extraction.  
- Preprocess images by resizing and flattening for SVM input.  
- Train a **linear SVM** classifier on the dataset.  
- Evaluate performance using **accuracy** and **classification report**.  
- Visualize:
  - Correctly classified images  
  - Misclassified images  
  - PCA scatter plot of the dataset  

## Requirements

- Python 3.x  
- Libraries: `numpy`, `opencv-python`, `matplotlib`, `scikit-learn`

## What the Script Does

The script performs the following steps:

1. **Load and preprocess images**  
   - Reads images directly from a ZIP file without extraction.  
   - Resizes all images to 64×64 pixels.  
   - Flattens images to prepare them for SVM input.  

2. **Train an SVM classifier**  
   - Uses a linear kernel to separate cats and dogs based on image features.  

3. **Display evaluation metrics**  
   - Computes and prints **accuracy** on the test set.  
   - Generates a **classification report** with precision, recall, and F1-score.  

4. **Visualize predictions**  
   - Shows a grid of **correctly classified images**.  
   - Shows a grid of **misclassified images**, highlighting prediction errors.  

5. **Generate a PCA scatter plot**  
   - Reduces high-dimensional image data to 2D using **Principal Component Analysis (PCA)**.  
   - Visualizes clusters of cats and dogs to inspect separability.

---

## Output

After running the script, you will get:

- **Accuracy** of the SVM classifier on the test set.  
- **Classification report** including precision, recall, and F1-score for each class.  
- **Visualizations**:  
  - Correctly classified images  
  - Misclassified images  
  - PCA scatter plot showing clustering of cats vs dogs  

---

## Notes

- PCA is used **only for visualization** to reduce 12,288-dimensional image vectors (64×64×3) to 2D.  
- The SVM classifier is trained on **flattened image vectors**.   

