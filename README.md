# Object-detection-for-whiteflies-monitoring-using-YOLOV8
## Why
Deep learning is widely applied in various fields and has achieved excellent results, assisting in the advancement of academia and industry. In agriculture, the cultivation management of crops directly affects the quality of fruits and vegetables, with pest and disease management being a particularly important aspect. Even advanced agricultural companies are troubled by pest and disease infestation. Therefore, it's urgent to introduce artificial intelligence to enhance monitoring efficiency, achieving the goal of early warning of pest and disease occurrence, reducing the economic losses. Here, a case about whiteflies monitoring using deep learning was studied.
## How
In this case, YOLOV8[1], as a SOTA algorithm was selected to conduct object detection. All images of whiteflies on yellow sticky traps were collected using the smartphone by the author[2]. The details were described below:
### Set up working environment
Install:
(1) Anaconda(A platform for managing python)
(2) CUDA(A package for GPU computing)
(3) Pytorch(A framework for Deep learning)
(*) Check https://blog.csdn.net/qq_45956730/article/details/126600028 for details.
### Prepare data
Collect images and labels as much as possible(put more efforts on this, the greater amount for data, the better performance for the model).
(*) LabelImg(https://github.com/HumanSignal/labelImg) and Roboflow(https://roboflow.com/) are recommendded to do this work.
### Model training 
(1)

## Note
1. For more information about YOLOV8, please check: https://docs.ultralytics.com/.
2. Feel free to use these images ^_^.
