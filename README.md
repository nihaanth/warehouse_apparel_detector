YOLOv5 Warehouse Apparel Detector

This repository contains a YOLOv5 object detection model trained on a custom dataset for detecting apparel in warehouse environments. The model is capable of detecting a range of apparel items, including shirts, pants, jackets, and more. The model has been optimized for use in warehouse environments, where apparel may be stacked on shelves or packed in boxes, making it difficult to manually track inventory.

Dataset

The dataset used to train this model consists of thousands of images of apparel in warehouse environments. The images were collected from a variety of sources, including publicly available datasets and images captured by warehouse employees. The images were labeled using the LabelImg tool to create bounding boxes around each apparel item.

Model

The YOLOv5 object detection model was trained using the PyTorch framework. The model consists of a backbone network, a neck network, and a head network. The backbone network is a modified version of the popular EfficientNet architecture, which has been shown to perform well on a wide range of computer vision tasks. The neck network consists of a series of convolutional layers that help to fuse information from different layers of the backbone network. The head network is responsible for predicting the location and class of each object in the input image.

Performance

The model has been evaluated on a test set of images and achieved an average precision of 0.85. The model is capable of detecting apparel items with high accuracy, even in cluttered environments where items may be partially occluded or stacked on top of each other.

Installation

To install and run the YOLOv5 Warehouse Apparel Detector, follow these steps:

Clone the repository:https://github.com/nihaanth/warehouse_apparel_detector.git

Usage

To use the YOLOv5 Warehouse Apparel Detector, simply run the detect.py script and provide the path to your input video file. The detector will process each frame of the video and output a new video file with bounding boxes around each detected apparel item. You can adjust the confidence threshold for detection by changing the value of --conf-thres (default value is 0.5).

Acknowledgments

This project was inspired by the YOLOv5 object detection framework developed by Ultralytics. The backbone network was adapted from the EfficientNet architecture developed by Google. The dataset used to train the model was sourced from a variety of publicly available datasets and images captured by warehouse employees.
