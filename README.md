# Water Segmentation Project

This project implements a **deep learning model for water segmentation** from multi-channel satellite images using PyTorch and the `segmentation_models_pytorch` library. Each image has **12 channels**, and the labels are **binary masks** indicating water vs. background.  

---

## Project Structure

- `data/images/` : Input images in TIFF format (12 channels each)  
- `data/labels/` : Ground truth masks in PNG format (binary masks)  
- `pre-trained.ipynb` : Jupyter notebooks for preprocessing, training, and visualization  


---

## Features

- Load and preprocess **multi-channel TIFF images** and corresponding masks.  
- Normalize input images and ensure labels are binary.  
- Train a **pretrained UNet model** (ResNet34 encoder) for segmentation.  
- Evaluate using **Dice coefficient, IoU, Precision, Recall, and F1-score**.  
- Visualize input images, true masks, and predicted masks.  

---

## Requirements

- Python 3.8+  
- PyTorch  
- segmentation_models_pytorch  
- numpy  
- matplotlib  
- tifffile  
- scikit-learn  
- Pillow  
- scikit-image  

Install dependencies using pip:

```bash
pip install torch torchvision segmentation-models-pytorch numpy matplotlib tifffile scikit-learn Pillow scikit-image
