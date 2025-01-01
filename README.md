# Guns-100-11m

## Model Overview

**Architecture:** YOLOv11  
**Training Epochs:** 100  
**Batch Size:** 32  
**Optimizer:** auto  
**Learning Rate:** 0.0005  
**Data Augmentation Level:** Moderate

## Training Metrics

- **mAP@0.5:** 0.85476

## Class IDs

| Class ID | Class Name |
|----------|------------|
| 0 | Gun |
| 1 | Knife |


## Datasets Used

- gun-detection-xwosb_v8
- gun-sqvhj_v1
- people_with_guns_2-pvcnk_v9
- police1_v1
- soldier-wclp7_v1
- test-e46au_v1
- weapon-rl8c4_v3
- weapondetection-fdzlo_v4
- weapons-detection-x9fnq_v3
- wepon_detection_v1

## Class Image Counts

| Class Name | Image Count |
|------------|-------------|
| Gun | 44219 |
| Knife | 4038 |


## Description

This model was trained using the YOLOv11 architecture on a custom dataset. The training process involved 100 epochs with a batch size of 32. The optimizer used was **auto** with an initial learning rate of 0.0005. Data augmentation was set to the **Moderate** level to enhance model robustness.

## Usage

To use this model for inference, follow the instructions below:

```python
from ultralytics import YOLO

# Load the trained model
model = YOLO('best.pt')

# Perform inference on an image
results = model('path_to_image.jpg')

# Display results
results.show()
