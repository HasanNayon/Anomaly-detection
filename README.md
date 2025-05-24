# Anomaly Detection using MVTec Anomaly Detection Dataset

This project focuses on implementing an **Anomaly Detection** system using the **MVTec Anomaly Detection (MVTec AD)** dataset. The goal is to detect defects or irregularities in images of various industrial objects and textures using deep learning and computer vision techniques.

## 📌 Project Overview

Anomaly detection is critical in industrial applications, where identifying defects can significantly impact quality assurance and production efficiency. This project aims to build a robust anomaly detection pipeline that can:

- Detect and localize visual defects in object and texture images.
- Differentiate between normal and defective samples.
- Provide visual insights for detected anomalies using segmentation maps.

## 📂 Dataset: MVTec AD

**MVTec AD** is a high-resolution dataset for benchmarking anomaly detection methods. It contains 15 categories including both objects (e.g., bottle, cable, capsule) and textures (e.g., grid, leather, tile).

- **Normal images**: Used for training (only normal images are used to learn the distribution).
- **Anomalous images**: Used for testing, include various types of defects.
- **Ground truth**: Pixel-wise segmentation masks for evaluating localization performance.

### 🔗 Dataset Link

You can download the dataset from the official MVTec website:  
[https://www.mvtec.com/company/research/datasets/mvtec-ad](https://www.mvtec.com/company/research/datasets/mvtec-ad)

## ⚙️ Project Structure

```bash
anomaly-detection/
├── data/
│   └── mvtec_ad/              # Contains the MVTec dataset
├── models/                    # Trained models or model checkpoints
├── notebooks/                 # colab notebooks for experiments and visualization
├── src/                       # Source code
│   ├── dataloader.py          # Dataset preprocessing and loading
│   ├── train.py               # Model training script
│   ├── test.py                # Model evaluation
├── outputs/                   # Results, segmentation maps, etc.
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
