# Object-detection-for-whiteflies-monitoring-using-YOLOV8
## Schematic diagram
<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/flowchart.jpg" width="400">

## Description
(1) Objective  
As a strategy of Integrated pest management (IPM), monitoring the occurence of pests helps to control them, preventing crops from severe loss. An efficient way to complete this task is applying deep learning (DL) to detecting pests (whiteflies, for this case).

<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/step1.jpg" width="300">

(2) Solution  
Object detection is considered as a powerful technique to recognize and locate the targets. Collecting the images was first step, then LabelImg and Roboflow were used to create labels and augment/split data, seperately. After completing the whole dataset, YOLO v8 was used to train models for whitefly detection.
(3) Results  


## Details for this work
### Set up working environment
Install:  
(1) Anaconda (An IDE for managing packages of python)  
(2) CUDA (A package for GPU computing)  
(3) Pytorch (A framework for Deep learning)  
(4) ultralytics (YOLOV8)  
For (1)~(3), check https://blog.csdn.net/qq_45956730/article/details/126600028 for details, then visit https://docs.ultralytics.com/ for more information about installation.
### Prepare data
(1) Collect images and labels. For images, Kaggle (https://www.kaggle.com/datasets?search=image) is an excellent platform to acquire various image datasets. For labels, LabelImg (https://github.com/HumanSignal/labelImg) and Roboflow (https://roboflow.com/) are recommendded to do this work.  
(2) Set up ".yaml" file. Find the "dataset" folder (Default path: C:\Users\User\anaconda3\envs\yolov8\Lib\site-packages\ultralytics\cfg\datasets, while "Users" might be replaced by your name), create a new blank .yaml file by adding a .txt file. The format of the new file should be similar to the others (like the "coco.yaml"), and the contents includes:  

path: path of images and labels  
train: path of training set  
val: path of validataion set  
nc: numbers of the classes  
names: the name of labels for images  

### Model training, validation, prediction and deployment
(1) 
