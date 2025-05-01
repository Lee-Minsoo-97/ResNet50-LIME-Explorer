# ResNet50 LIME Explorer

_Visualizing and Interpreting ResNet50 Predictions with LIME_

---

## Overview
**ResNet50 LIME Explorer** is a lightweight framework that demonstrates how to generate and visualize local explanations for image-classification decisions made by a pre-trained ResNet50 model using LIME (Local Interpretable Model-agnostic Explanations). By isolating superpixels and showing their positive or negative influence, this project helps you understand which image regions drive the network’s top predictions.

## Features
- Load any input image and classify it with ResNet50 (ImageNet weights).  
- Generate LIME explanations highlighting influential superpixels.  
- Overlay positive/negative contributions on the original image.  
- Produce an RdBu heatmap showing segment-level contributions.  
- Minimal dependencies—only TensorFlow, Keras, LIME, and Matplotlib.

## Requirements
- Python 3.7+  
- `tensorflow`  
- `tensorflow_datasets`  
- `keras`  
- `numpy`  
- `matplotlib`  
- `lime`  
- `scikit-image`

## Installation
```bash
pip install tensorflow tensorflow_datasets keras numpy matplotlib lime scikit-image
