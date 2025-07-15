# 🚁 Small Object Detection in Aerial Videos using YOLOv8

Author:Premnath MV  
Reg No:URK23RA4014


---

## 📌 Project Description

This project focuses on detecting **small objects Detectiton** in aerial videos using the **YOLOv8** deep learning model. The goal is to improve detection accuracy for small targets like pedestrians, bicycles, and cars in drone footage using the **VisDrone dataset**.

---

## 🛠️ Tools and Technologies

- Python
- YOLOv8 (Ultralytics)
- OpenCV
- PyTorch
- VisDrone Dataset
- Command Line

---

## 🔧 Setup Instructions

### 1. Clone YOLOv8 repository

```bash
git clone https://github.com/ultralytics/ultralytics
cd ultralytics
pip install -r requirements.txt

## 📂 Dataset Structure

This project uses the **VisDrone** dataset, converted into YOLO format. Ensure your folders are organized as shown below before training:

VisDrone-YOLO/
├── images/
│ ├── train/
│ └── val/
├── labels/
│ ├── train/
│ └── val/
└── data.yaml

