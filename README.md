<img width="1920" height="1080" alt="sample_image" src="https://github.com/user-attachments/assets/87bd5639-44fa-4e3d-b86d-136b27fa01e0" />
# Real-Time Traffic Density Estimation using YOLO11

**An advanced computer vision solution for real-time vehicle detection and dual-lane traffic density estimation using YOLO11 Nano and OpenCV.**

---

## 🌟 Features

- **State-of-the-art Vehicle Detection** with **YOLO11 Nano**
- **Real-time Traffic Intensity Analysis** (Smooth / Heavy)
- **Dual-lane ROI-based Counting** using OpenCV polygon regions
- **High Accuracy**: 97.4% mAP50 | 94.7% Recall | 91.2% Precision
- **ONNX Export** ready for deployment (C++ / OpenCV)
- **Interactive Dashboard** showcasing results, metrics, and video inference
- **Comprehensive EDA** and training visualization

---

## 📊 Project Overview

This project implements an end-to-end pipeline for estimating traffic density from top-view highway camera feeds. The system detects vehicles using a custom-trained **YOLO11** model and classifies them into left and right lanes using predefined polygonal regions of interest (ROI).

**Key Achievements:**
- Successful migration from YOLOv8 to **YOLO11**
- Training completed in ~30 minutes on GTX 1650 with CUDA
- Robust handling of Windows Unicode paths
- Clean dataset with zero annotation errors

---

## 🛠️ Tech Stack

| Component              | Technology                          |
|------------------------|-------------------------------------|
| Object Detection       | YOLO11 Nano (Ultralytics)           |
| Computer Vision        | OpenCV                              |
| Training               | PyTorch + CUDA                      |
| Model Export           | ONNX                                |
| Visualization          | Matplotlib, Seaborn                 |
| Dashboard              | HTML + CSS + JavaScript             |
| Notebooks              | Jupyter Notebook                    |

---

## 📁 Project Structure

```bash
Traffic-Density-Estimation/
├── runs/detect/train/              # Training results (Ultralytics)
│   ├── results.png
│   ├── confusion_matrix_normalized.png
│   └── BoxPR_curve.png
├── eda_box_distributions.png
├── processed_sample_video.mp4
├── best.onnx                       # Exported model (10.1 MB)
├── Traffic_Density_Advanced_Modeling.ipynb
├── Traffic_Density_Advanced_EDA.ipynb
├── Traffic_Density_Estimation_Portfolio.html  # Main Dashboard
├── assets/                         # Screenshots & extra media
└── README.md

📈 Results

mAP50: 97.4%
mAP50-95: 72.4%
Precision: 91.2%
Recall: 94.7%
Strong performance even under shadows and glare

🧪 Dataset

Total Images: 626 (640×640)
Train: 536 images (with horizontal flip augmentation)
Validation: 90 images
Class: Vehicle (single class)
Format: YOLOv8 label format

🔧 How to Run
  Clone the repository:
git clone https://github.com/yourusername/Traffic-Density-Estimation.git
cd Traffic-Density-Estimation

Open the dashboard:
# Just open the HTML file in any browser

For inference (Python):
pip install ultralytics opencv-python
python inference.py    # (You can add your script)

📌 Future Improvements

 Multi-camera support
 Speed estimation (km/h)
 Web deployment (FastAPI + WebSocket)
 Vehicle type classification (Car, Truck, Bus, etc.)
 Edge deployment on NVIDIA Jetson

👨‍💻 Author
Ali Naderi
AI Engineer & Data Scientist

Portfolio: file:///D:/Work%20Space/%D9%81%D8%B5%D9%84%20%DA%86%D9%87%D8%A7%D8%B1%D9%85/Real-Time%20traffic%20density%20estimation/Traffic_Density_Estimation_Portfolio.html
LinkedIn: www.linkedin.com/Alinaderi1

📄 License
This project is open for educational and portfolio purposes. Feel free to use it as inspiration.

Made with ❤️ using YOLO11
