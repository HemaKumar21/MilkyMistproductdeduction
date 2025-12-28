MilkyMist Product Detection using YOLOv8
Project Status: In Progress

This project focuses on detecting MilkyMist dairy products from images using a deep learning–based object detection approach.
The solution is built using the YOLOv8 model to identify different product categories such as curd, milkshake, and paneer.

The project is currently under active development, with continuous improvements planned in dataset quality, model performance, and deployment.

Problem Statement

Manual identification and classification of dairy products from images can be inefficient and error-prone.
This project aims to automate product identification using computer vision techniques, which can be applied to:

Retail shelf monitoring

Inventory management

Smart billing systems

Quality control in dairy manufacturing

Solution Overview

Implemented a YOLOv8-based object detection pipeline

Trained the model on a custom-labeled MilkyMist product dataset

Performed training and validation using GPU acceleration in Google Colab

Evaluated performance using standard object detection metrics

Technology Stack

Programming Language: Python

Deep Learning Framework: PyTorch

Model Architecture: YOLOv8 (Ultralytics)

Libraries: OpenCV, NumPy, Matplotlib

Development Environment: Google Colab

Project Structure
MilkyMistproductdeduction/
│
├── MilkyMistproductdeduction.ipynb   # Model training and inference
├── data/
│   ├── train/
│   ├── valid/
│   └── data.yaml
├── runs/                             # YOLO training outputs
├── README.md

Installation and Setup

Install the required dependency:

pip install ultralytics


Import the YOLO model:

from ultralytics import YOLO


A GPU-enabled environment is recommended for training.

Model Training Details (Current)

Base model: yolov8s.pt (pretrained)

Number of classes: 3

Curd

Milkshake

Paneer

Image size: 640 × 640

Training epochs: 100 (with early stopping)

Current Results

The model successfully detects MilkyMist products in images

Performance is currently limited due to:

Small dataset size

Class imbalance

Limited image diversity

The results shown are preliminary and will improve with further iterations.

Future Development

Planned enhancements include:

Expanding the dataset with more real-world images

Adding additional MilkyMist product categories

Improving annotation quality and consistency

Hyperparameter tuning for improved accuracy

Real-time product detection using live camera feeds

Web-based deployment using Flask or FastAPI

Integration with mobile or edge devices

Detailed performance analysis and visualization

Contributions

This project is maintained by Hema Kumar V.
Contributions and suggestions can be considered once the core implementation is completed.

Disclaimer

This project is developed for academic and learning purposes and is not officially affiliated with MilkyMist.
