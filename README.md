# Object-Detection-using-Deep-Learning-OpenCV-and-Powerful-Python-Libraries
This project utilizes the Deep Learning model ( YOLOv3-tiny model ) for object detection in images , video and real time using Python and OpenCV.

This repository contains code for object detection using YOLOv3 (You Only Look Once version 3) with OpenCV and Python. YOLO is an object detection algorithm that stands for "You Only Look Once". It's known for its speed and accuracy in detecting objects in images and videos.

## Prerequisites
Before running the code, make sure you have the following installed:

Python 3.x
OpenCV
NumPy
Matplotlib

## Usage
You also need to download the YOLOv3 weights, configuration file, and the COCO dataset class names file. You can find these files from the official YOLO website or other sources, OR you can download it from my repository too!

### YOLOv3 Tiny Weights:
YOLOv3 Tiny is a lighter version of the YOLO (You Only Look Once) object detection algorithm.
The weights file contains pre-trained weights for the YOLOv3 Tiny model, which have been trained on a large dataset (such as COCO).
These weights are used to initialize the neural network architecture of YOLOv3 Tiny during inference, allowing it to detect objects in images with high accuracy.

### Configuration File:
The configuration file (yolov3-tiny.cfg) contains the architecture or configuration of the YOLOv3 Tiny neural network.
It specifies details such as the number of layers, filter sizes, strides, and other parameters that define the network's architecture.
The configuration file is essential for loading the correct architecture when initializing the YOLOv3 Tiny model during inference.

### COCO Dataset Class Names File:
The COCO (Common Objects in Context) dataset is a large-scale dataset that contains images with objects from 80 different classes.
The class names file (coco.names) contains a list of these 80 class names, each corresponding to a specific object category.
During object detection, the model uses this file to map the class indices predicted by the network to their corresponding class names, making it easier to interpret the results.
These files are crucial components for performing object detection using YOLOv3 Tiny. Make sure to download or obtain these files from reliable sources before running your object detection code.

#### Official YOLO Website-YOLO: Real-Time Object Detection.
#### COCO Dataset Website-COCO - Common Objects in Context.

## Object Detection in images 
The detect_objects function takes an image as input and returns a list of detected objects along with their bounding boxes and confidences.

(Parameter) img: Input image (numpy array) where objects are to be detected.

#### detected_objects:
A list containing dictionaries for each detected object. Each dictionary contains the following keys:
##### class_id:The ID of the detected object class.
##### confidence: The confidence score of the detection.
##### box: The bounding box coordinates of the detected object in the format [x, y, w, h].

This code will draw bounding boxes around detected objects on the original image and display the result using OpenCV.

## Object Detection in Real Time
In this we are trying to capture video from an IP camera or machine camera using OpenCV, detect objects in each frame using a function called detect_objects, and then save the processed video to a file.

### For IP camera access  
Make sure to replace "URL corresponds to a webcam feed" with the actual URL of your IP camera stream.

Given code (object detection using Machine camera ( Real Time ).ipynb) will capture video from the provided URL, detect objects in each frame using the detect_objects function, draw bounding boxes around detected objects, save the processed video and display the processed video in a window.

### For Machine camera access 
Given code (object detection using webcam ( Real Time ).ipynb) captures video from the webcam, processes each frame to detect objects using the detect_objects function, and displays the processed video in a window. 

