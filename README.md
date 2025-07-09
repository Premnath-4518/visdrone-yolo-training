# VisDrone Object Detection using YOLOv5

This repository contains my work on training a YOLOv5 model to detect **80 object classes** from aerial imagery using the **VisDrone dataset**.

## 🔧 Setup Instructions

```bash
# Clone YOLOv5 repository
git clone https://github.com/ultralytics/yolov5
cd yolov5

# Install dependencies
pip install -r requirements.txt

I used the VisDrone dataset with 80 classes, converted to YOLO format. Make sure your folder structure is like this:

kotlin
Copy
Edit
VisDrone-YOLO/
├── images/
│   ├── train/
│   └── val/
├── labels/
│   ├── train/
│   └── val/
└── data.yaml
Example data.yaml
yaml:
train: C:/Users/VisDrone-YOLO/VisDrone-YOLO/VisDrone-YOLO/images/train
val: C:/Users/VisDrone-YOLO/VisDrone-YOLO/VisDrone-YOLO/images/val

nc: 80
names: [person, bicycle, car, motorcycle, airplane, bus, train, truck, boat, traffic light, ...]

🚀 Training Command

python train.py --img 640 --batch 16 --epochs 30 --data data.yaml --weights yolov5s.pt --name visdrone_run

🔍 Inference Command
bash
python detect.py --weights runs/train/visdrone_run/weights/best.pt --img 640 --conf 0.25 --source C:/Users/VisDrone-YOLO/VisDrone-YOLO/VisDrone-YOLO/images/val

📈 Results
Training and validation logs are saved in: runs/train/visdrone_run

TensorBoard:
bash
tensorboard --logdir runs/train

🙋‍♂️ Author
Premnath
2nd Year – B.Tech Robotics and Automation
Karunya Institute of Technology and Sciences


