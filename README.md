# YOLOv8 Object Detection Application

## Overview

This project implements an object detection system using the YOLOv8 deep learning model. It can detect and label multiple objects in images and videos with bounding boxes and class names.

The system supports:

- Image detection with visual bounding boxes  
- Video detection processing frames one by one  
- Optional resizing and confidence threshold tuning for better performance

---

## Features

- Uses Ultralytics YOLOv8 pretrained models (`nano`, `medium`, `large`)  
- Supports image and video file uploads for detection  
- Displays annotated images and saves processed videos  
- Runs on Google Colab (with GPU) or local Python environment  
- Utilizes OpenCV for image/video processing and Matplotlib for visualization

---

## Installation

### On Local Machine

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/yolov8-object-detection.git
   cd yolov8-object-detection
Usage
Image Detection
Upload an image file.

The system will detect objects and display annotated bounding boxes with labels.

Confidence threshold can be adjusted to control detection sensitivity.

Video Detection
Upload a video file.

The system processes frames one-by-one, detects objects, and saves an annotated output video.

The output video can be downloaded after processing.

Model Options and Performance
Model	Accuracy vs Speed
YOLOv8 Nano	Fastest, less accurate
YOLOv8 Medium	Balance of speed and accuracy
YOLOv8 Large	Most accurate, slowest

Recommendation: Use smaller models like nano or medium for faster iteration, and large for final evaluation if hardware allows.

Dependencies
Python 3.8+

ultralytics (YOLOv8)

opencv-python / opencv-python-headless

matplotlib

streamlit (optional, for UI deployment)

Notes
Large models may run slowly on free GPUs (e.g., Google Colab).

Resize images to 640x640 for faster inference.

Action recognition (e.g., "cleaning glasses") is outside the scope of YOLO object detection.
