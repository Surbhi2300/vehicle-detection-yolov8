# Vehicle Detection using YOLOv8

## Overview
This project implements a multi-class vehicle detection system using YOLOv8.
The model detects vehicles such as cars, buses, trucks, auto-rickshaws, etc.
from road traffic images and videos.

## Why this project?
Vehicle detection is a core computer vision problem used in:
- Traffic monitoring
- Smart cities
- Road safety
- Intelligent transportation systems

This project demonstrates a complete end-to-end ML pipeline.

## Dataset
- Dataset sourced from Roboflow
- Pre-annotated vehicle dataset (YOLO format)
- 15 vehicle classes
- Dataset not included in repository due to size constraints

## Model
- YOLOv8 (Ultralytics)
- Transfer learning using COCO pretrained weights
- Trained on custom dataset

## How the project works
1. Dataset selection and annotation (Roboflow)
2. Model training using YOLOv8
3. Model evaluation
4. Image and video inference

## How to run

### Install dependency
pip install ultralytics

### Image detection
yolo detect predict model=models/best.pt source=data/raw_images


### Video detection
yolo detect predict model=models/best.pt source=data/raw_videos

## Results
- Bounding boxes around vehicles
- Class labels and confidence scores
- Works on real-world traffic data

## Notes
- Training outputs and datasets are excluded using .gitignore
- Trained model can be shared separately if required

## Author
Surbhi Aglawe