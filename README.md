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
- Jupyter Notebook / Command Line

---

## 🔧 Setup Instructions

### 1. Clone YOLOv8 repository

```bash
git clone https://github.com/ultralytics/ultralytics
cd ultralytics
pip install -r requirements.txt

### 2. Prepare VisDrone Dataset (YOLO format)
### Make sure your folder structure is like this:

VisDrone-YOLO/
├── images/
│   ├── train/
│   └── val/
├── labels/
│   ├── train/
│   └── val/
└── data.yaml


