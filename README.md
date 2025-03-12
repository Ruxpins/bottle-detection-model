# Plastic Bottle Detection Model
#***these instructions are not complete***

This repository contains a YOLOv8 model trained to detect plastic bottles in images. The model was trained on a custom dataset using the Ultralytics YOLOv8 framework. It is relatively small in size so it can be used on a Sony IMX500 image sensor.

## Model Details
- Base Model: YOLOv8n
- Training Dataset: Plastic Bottle Image Dataset
- Training Duration: 50 epochs
- Best Performance Metrics:
  - Precision: 0.694 (69.4%)
  - Recall: 0.498 (49.8%)
  - mAP50: 0.496 (49.6%)
  - mAP50-95: 0.339 (33.9%)

## Usage
1. Install requirements:
   bash
   pip install ultralytics

2. Download the model weights and use them with YOLOv8:
   from ultralytics import YOLO
   model = YOLO('best.pt')
   results = model.predict('your_image.jpg')

## Project Structure
- \data.yaml\: Dataset configuration file
- \test.pt\: Best model weights (available in releases)
- \train.py\: Training script
