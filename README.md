# BloodCellDetection_YOLO

This repository is an implemetation of YOLO1 for blood cell detection, 2 class of cell are present : rbc, wbc\
I used the architecture described in the paper.
The repository includes:
- Dataset : image folder + annotation csv file
- jupyter notebook containing all the steps: data loding ,data preprocessing, training, testing
- Pre-trained weights

## DATASET
you can find the bloodcell dataset from kaggle, it containes an images directory and annotation csv file of the bouding boxes coordinates.

Here is an example of the annotated dataset:\
<img src="/assets/dataset_image_example.PNG"  width="600" height="600"/> 

https://www.kaggle.com/draaslan/blood-cell-detection-dataset

## TRAINING
The architecture used is a reduced architecture of the one explained in the paper (only one conv layer was removed)
![GitHub Logo](/assets/architecture.PNG)

Hyperparemeters :
- image size = 224
- learning rate = 2e-5
- batch size = 1 # 64 in original paper
- epochs = 100

Loss function and optimizer:
- Adam optimizer
- loss function as described in the iriginal paper in the reference \
![GitHub Logo](/assets/loss_function.PNG)



## RESULT
The model reach in 100 epochs:
- Mean loss of 4.45
- mean average precision (MAP) of 0.86 

![GitHub Logo](/assets/map.PNG)

Here is the result of the YOLOv1 bloodcell detection.\
![GitHub Logo](/assets/Result.PNG)

The blood cell detection was almost perfect, I believe if I did train it for some more time it will perform perfect detections


#### REFERENCES
You Only Look Once: Unified, Real-Time Object Detection, https://pjreddie.com/media/files/papers/yolo.pdf
