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

### Project Structure
├── Assignment_5_LIME–Framework.py    # Main script with framework cells
├── README.md                         # This file
└── images/                           # (Optional) example input images

### Usage
	1.	**Prepare your image**
Upload a clear, single-object photo (e.g., animal, car, appliance).
	2.	**Set image_path**
In the “EDIT THIS CELL” section of Assignment_5_LIME–Framework.py, update:
image_path = '/path/to/your/image.jpg'
	3.	Run the script/notebook
  	•	Execute all cells in order.
  	•	The framework will:
	    1.	Predict the top 3 ImageNet classes with ResNet50.
	    2.	Create a LimeImageExplainer and explain the top label.
	    3.	Display:
	      •	An overlay of all positive & negative superpixels.
      	•	A second overlay showing only positive contributions.
      	•	An RdBu heatmap of segment-wise weights.
	4.	Interpret results
	  •	Green outlines: selected superpixels (pos & neg).
	  •	Black areas: segments not used in explanation.
	  •	Blue vs. red (heatmap): positive vs. negative contributions.



## References
	•	Ribeiro, M. T., Singh, S., & Guestrin, C. (2016). “Why Should I Trust You? Explaining the Predictions of Any Classifier.”
	•	LIME Documentation. https://lime-ml.readthedocs.io/en/latest/
	•	TensorFlow ResNet50 Tutorial. https://www.tensorflow.org/api_docs/python/tf/keras/applications/ResNet50
