# BloodCellDetection_YOLO

This repository is an implemetation of YOLO1 for blood cell detection, 2 class of cell are present : rbc, wbc
we used thr architecture described in the paper.

## DATASET
you can find the bloodcell dataset from kaggle, it containes an images directory and annotation csv file of the bouding boxes coordinates.

Here is an example of the annotated dataset:\
<img src="/images/dataset_image_example.PNG"  width="600" height="600"/> 

https://www.kaggle.com/draaslan/blood-cell-detection-dataset

## TRAINING
The architecture used is a reduced architecture of the one explained in the paper (only one conv layer was removed)
![GitHub Logo](/images/architecture.PNG)

Hyperparemeters :
- image size = 224
- learning rate = 2e-5
- batch size = 1 # 64 in original paper
- epochs = 100
Loss function and optimizer:
- Adam optimizer
- b


## RESULT
The model reach in 100 epochs:
- Mean loss of 4.45
- mean average precision (MAP) of 0.86 

Here is the result of the YOLOv1 bloodcell detection.
![GitHub Logo](/images/Result.PNG)

The blood cell detection was almost perfect, I believe if I did train it for some more time it will perform perfect detections


#### REFERENCES
You Only Look Once: Unified, Real-Time Object Detection, https://pjreddie.com/media/files/papers/yolo.pdf
