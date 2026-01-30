# Object Recognition System using Deep Learning
WiDS Course Project
This repository contains a complete computer vision pipeline developed over four weeks. The system leverages YOLOv5 for real-time pedestrian detection and DeepSORT for multi-object tracking, specifically designed to identify abnormal movement patterns in public spaces.

Project Roadmap & Learnings
Phase 1: CNN Theory & Object Detection (Week 1 & 2)
We started by exploring the mathematical foundations of Convolutional Neural Networks, focusing on spatial feature extraction. I implemented the YOLOv5 architecture, which allows for single-pass inference, making it ideal for real-time surveillance applications.

Phase 2: Custom Training on MOT17 (Week 3)
I trained a custom detector using the Multiple Object Tracking 2017 (MOT17) dataset. This involved:

Converting raw CSV annotations into normalized center-based coordinates.
Fine-tuning the YOLOv5m model by freezing backbone layers to utilize transfer learning from the COCO dataset.

Phase 3: Tracking & Anomaly Detection (Week 4)
Using the DeepSORT algorithm, I integrated temporal tracking to assign unique IDs to pedestrians. The system includes an anomaly engine that calculates velocity vectors and displacement to flag irregular behaviors, such as running or entering forbidden zones.

