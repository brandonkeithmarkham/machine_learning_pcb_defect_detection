# 🖼️ PCB Defect Detection with Transfer Learning

This repository contains the source code, datasets, and documentation for a project exploring the use of **object detection and transfer learning** to automatically detect defects in Printed Circuit Boards (PCBs). The project evaluates three state-of-the-art models: **YOLOv8, SSD MobileNet, and Faster R-CNN**, trained and tested on an augmented PCB dataset:contentReference[oaicite:0]{index=0}.

## 📄 Project Overview
The goal of this project was to automate PCB defect detection, traditionally performed by manual visual inspection. Using object detection models and transfer learning, we trained models on a dataset of defective and non-defective PCB images to compare their performance in terms of accuracy, precision, recall, and mean average precision (mAP).  

## 🛠 Tools & Methods
- **Frameworks**: PyTorch (YOLOv8), TensorFlow (SSD MobileNet, Faster R-CNN)  
- **Techniques**: Transfer learning, data augmentation (rotations, class balancing)  
- **Visualization**: t-SNE and UMAP for class separability  
- **Dataset**: 1,636 images across 7 classes (defective + non-defective), annotated in Pascal VOC XML format:contentReference[oaicite:1]{index=1}  
- **Models Implemented**:
  - **YOLOv8** (one-stage, real-time detector)  
  - **SSD MobileNet** (lightweight, resource-efficient)  
  - **Faster R-CNN** (two-stage, accurate but computationally intensive)  

## 📊 Key Outcomes
- **YOLOv8**: Best overall, achieving **97.2% mAP**, with precision = 96.1% and recall = 96%:contentReference[oaicite:2]{index=2}  
- **Faster R-CNN**: High accuracy (**mAP = 95.7%**) but slower and more resource-intensive  
- **SSD MobileNet**: Fastest and most lightweight, but performed poorly (**mAP = 27%**) making it unsuitable for high-accuracy applications  
- Demonstrated the **practicality of transfer learning** for defect detection with limited datasets  

## 📄 Documentation
The full paper, including methodology, experimental results, and visualizations, can be found here:  
👉 [**Final Report**](./docs/PCB_Defect_Detection_Paper.pdf)  

## 🔖 Notes
- The dataset was augmented to address class imbalance and increase robustness.  
- TFRecords and YOLOv8-style annotations were generated for compatibility with different frameworks.  
- Future work includes dataset expansion, noise augmentation, model optimization, and testing newer detectors like YOLOv9:contentReference[oaicite:3]{index=3}.  

## 📝 Authors
Brandon Markham, John Gellerup, Josh Muniga  

## 📫 Contact
[LinkedIn](https://www.linkedin.com/) | [Email](mailto:youremail@example.com)
