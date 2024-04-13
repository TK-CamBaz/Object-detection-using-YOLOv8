# Object-detection-for-whiteflies-monitoring-using-YOLOV8
## Schematic diagram
<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/flowchart.jpg" width="400">

## Description for each item

## Set up working environment
Install:  
(1) Anaconda (An IDE for managing packages of python)  
(2) CUDA (A package for GPU computing)  
(3) Pytorch (A framework for Deep learning)  
(4) ultralytics (YOLOV8)  
For (1)~(3), check https://blog.csdn.net/qq_45956730/article/details/126600028 for details, then visit https://docs.ultralytics.com/ for more information about installation.
## Prepare data
(1) Collect images and labels. For images, Kaggle (https://www.kaggle.com/datasets?search=image) is an excellent platform to acquire various image datasets. For labels, LabelImg (https://github.com/HumanSignal/labelImg) and Roboflow (https://roboflow.com/) are recommendded to do this work.  
(2) Set up ".yaml" file. Find the "dataset" folder (Default path: C:\Users\User\anaconda3\envs\yolov8\Lib\site-packages\ultralytics\cfg\datasets, while "Users" might be replaced by your name), create a new blank .yaml file by adding a .txt file. The format of the new file should be similar to the others (like the "coco.yaml"), and the contents includes:  

path: path of images and labels  
train: path of training set  
val: path of validataion set  
nc: numbers of the classes  
names: the name of labels for images  

## Model training, validation, prediction and deployment
(1) 

## Note
1. For more information about YOLOV8, please check: https://docs.ultralytics.com/.
2. Feel free to use these images ^_^.
