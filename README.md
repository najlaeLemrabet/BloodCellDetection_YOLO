# BloodCellDetection_YOLO

This repository is an implemetation of YOLO1 for blood cell detection, 2 class of cell are present : rbc, wbc
we used thr architecture described in the paper.
![GitHub Logo](/images/architecture.PNG)

## Dataset
you can find the bloodcell dataset from kaggle, it containes an images directory and annotation csv file of the bouding boxes coordinates.

Here is an example of the annotated dataset:\
<img src="/images/dataset_image_example.PNG"  width="600" height="600"/> 

https://www.kaggle.com/draaslan/blood-cell-detection-dataset




### Hyperparemeters :
IMG_SIZE = 224

LEARNING_RATE = 2e-5

BATCH_SIZE = 1 # 64 in original paper

EPOCHS = 100

The model reach a loss of Mean loss of 4.45 amd mean average precision (MAP) of 0.86 in only 100 epochs
Here is the result of the YOLOv1.
![GitHub Logo](/images/Result.PNG)



The blood cell detection was almost perfect, I believe if I did train it for some more time it will perform perfect detections


#### Ref :
You Only Look Once: Unified, Real-Time Object Detection, https://pjreddie.com/media/files/papers/yolo.pdf
