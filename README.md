# Boat Detection in Satellite Imagery with YOLOv8

This project builds an end-to-end pipeline for detecting boats in satellite imagery using a fine-tuned YOLOv8 model.  
The dataset is provided as NumPy arrays and normalized bounding boxes; it is converted into the YOLO format, used to train a custom detector, and evaluated through both CSV predictions and visual inspection.

## Project Overview

- Convert the raw training set into the YOLO directory structure  
- Train/validation split and label export (`.txt` files)  
- Fine-tune YOLOv8n on the custom boat dataset  
- Generate predictions on the test set (`predictions.csv`)  
- Visualize detections on unseen images  

This notebook can serve as a clean reference for training YOLO models on custom datasets.

## Results

The fine-tuned model achieves consistent detection of boats in the test images, including small and high-contrast objects typical of satellite views.  
Qualitative examples are available at the end of the notebook.

## Repository Structure

├── notebook.ipynb          # Complete training + prediction pipeline
├── predictions.csv         # Model output on the test set
├── boat_dataset_yolo/      # Generated YOLO-format dataset
└── README.md

