# RISE Saliency Maps for COCO Images

This repository contains a PyTorch implementation of **RISE** (Randomized Input Sampling for Explanation) for visualizing saliency maps of images from the COCO dataset. The notebook demonstrates how to generate importance maps, compute deletion and insertion metrics, and visualize the results.

---

## Project Overview

RISE is a black-box explanation method that highlights the regions in an input image that most influence a model’s prediction. Key components in this project:

- **Random mask generation** with upsampling and random shifts  
- **Black-box mask probing** → weighted aggregation → saliency map  
- **Deletion metric** – measures how prediction probability decreases as important pixels are removed  
- **Insertion metric** – measures how prediction probability increases as important pixels are added  
- **Visualization of saliency maps** with overlaid heatmaps  
- **Optional pointing game accuracy evaluation** (if ground truth masks are available)

---

## Requirements

- Python 3.8+  
- PyTorch  
- torchvision  
- PIL / Pillow  
- matplotlib  
- numpy  
- tqdm  

Install dependencies using pip:

```bash
pip install torch torchvision pillow matplotlib numpy tqdm
