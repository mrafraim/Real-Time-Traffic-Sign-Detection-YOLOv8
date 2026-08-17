# Real-Time Traffic Sign Detection Using YOLOv8

A multi-class traffic sign detection system built with YOLOv8, covering
dataset analysis, annotation validation, model training, evaluation,
error analysis, image inference, and video detection.

## Overview

This project develops a multi-class traffic sign detection system using
the YOLOv8 object detection framework.

The project follows an end-to-end computer vision workflow, beginning
with dataset exploration and annotation validation and progressing through
model training, evaluation, error analysis, image inference, and video
detection.

The final model is capable of detecting and classifying 15 traffic-sign
categories from visual input.

## Dataset

The project uses the [Traffic Sign Detection Dataset](https://www.kaggle.com/datasets/pkdarabi/cardetection)
available on Kaggle.

The dataset contains:

- **15 traffic-sign classes**
- **3,530 training images**
- **801 validation images**
- **638 test images**
- Images are provided at **416 × 416 pixels**

### Classes

| Category | Classes |
|---|---|
| Traffic Lights | Green Light, Red Light |
| Speed Limits | 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120 |
| Other | Stop |

## Exploratory Data Analysis

The dataset was analyzed to understand class distribution, objects per
image, image dimensions, and bounding-box characteristics before training.

![Dataset Distribution](assets/dataset_distribution.png)

All images share a consistent 416 × 416 resolution, while the bounding-box
analysis revealed the presence of very small objects that can be challenging
for detection.
