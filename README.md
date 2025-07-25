Road Sign Detection using YOLOv8
This project implements a real-time road sign detection system using YOLOv8, a state-of-the-art object detection model. The goal is to accurately detect and classify traffic signs in images or video streams.

🔍 Overview
Model: YOLOv8 (You Only Look Once - Version 8)

Type: Anchor-Free Object Detector

Use-case: Real-time road sign detection

Framework: PyTorch with Ultralytics YOLOv8


 Dataset
This project uses the **Self Driving Cars** dataset from [Roboflow](https://roboflow.com/), tailored for traffic object detection tasks.

- **Dataset Source**: Roboflow Universe  
- **Project**: Self Driving Cars  
- **Workspace**: `selfdriving-car-qtywx`  
- **Project ID**: `self-driving-cars-lfjou`  
- **Version**: 6 (YOLOv8 format)  
- **Dataset Link**: [Self Driving Cars v6 on Roboflow](https://universe.roboflow.com/selfdriving-car-qtywx/self-driving-cars-lfjou)

### Dataset Highlights
- Thousands of labeled images containing road signs, traffic lights, vehicles, pedestrians, etc.
- Available in YOLOv8 format for seamless integration with Ultralytics models.
- Ideal for both fine-tuning and training from scratch.


⚙️ Model Used
YOLOv8 Highlights:
Anchor-Free: Unlike older YOLO versions, YOLOv8 does not rely on predefined anchor boxes. Instead, it directly predicts object locations, improving performance and simplifying training.

Backbone: CSPDarknet

Neck: PANet

Head: Detection head with classification and bounding box regression

Export Options: ONNX, TorchScript, CoreML, TFLite

We used a pre-trained YOLOv8 model (e.g., yolov8n.pt, yolov8s.pt) and fine-tuned it on the road sign dataset using transfer learning.
