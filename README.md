# Object detection for whiteflies monitoring using YOLOv8
## Schematic diagram
<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/flowchart.jpg" width="400">

## Description
(1) Objective  
As a strategy of Integrated pest management (IPM), monitoring the occurence of pests helps to control them, preventing crops from severe loss. An efficient way to complete this task is applying deep learning (DL) to detecting pests (whiteflies, for this case).

<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/1.objective.jpg" width="300">

(2) Solution  
Object detection is considered as a powerful technique to recognize and locate the targets. Collecting the images was first step, then LabelImg and Roboflow were used to create labels and augment/split data, seperately. After completing the whole dataset, YOLOv8 was used to train models for whitefly detection.

<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/2.solution.jpg" width="500">

(3) Results  
Four models (yolov8x, yolov8x-p2, yolov8x-ghost and yolov8x-ghost-p2) were compared after training with the pre-traind weight (yolov8x.pt). In the following table, it's obvious that yolov8x-p2 had the highest precision and mAP50-95, and yolov8x-ghost-p2 had the highest recall and mAP50.

<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/Metrices.jpg" width="500">

The most comprehensible part of a object detection project is the visualization. Here, two images were selected to display the prediction performance of models. First image contained "relative large" whitefly samples, and second contained "relative tiny" ones. In the comparison of the prediction pattern, the four models detected most samples on both images, while a few blurred and tiny samples weren't detected.

<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/visual-large.jpg" width="500"> 
   
<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/visual-tiny.jpg" width="500">

In addition to the location of bounding boxes, the confidence score of bounding boxes was considered as a crucial role to describe the detection reliability of the model. The following boxplot figure indicated that the models showed little diffrence of confidence score for large samples, however, Y8G (the yolov8-ghost) model slightly outperfomed other models for tiny samples, which suggested it's more potential for this task.

<img src="https://github.com/TK-CamBaz/Object-detection-for-whiteflies-monitoring-using-YOLOV8/blob/main/Outline/Confidence.comparison.jpg" width="350">

### Reference
https://blog.csdn.net/qq_45956730/article/details/126600028 --> Set up working environment.  
https://docs.ultralytics.com/ --> YOLOv8 official website.  
https://www.kaggle.com/datasets?search=image --> A platform to acquire various image datasets.  
https://github.com/HumanSignal/labelImg --> A tool for creating labels for images.  
https://roboflow.com/ --> An online platform for storing, splitting and augmenting image data.  

### Note
The data and models are available in this repo, feel free to use, re-trained or reproduce results.
