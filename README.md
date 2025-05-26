# 🎥 Activity Detection Web Application

An interactive Streamlit-based computer vision application for real-time activity analysis using webcam input. This system integrates various features like **motion detection**, **object detection**, **pose estimation**, **intrusion alert**, and **face mesh rendering**—all presented in a clean UI with animated feedback.

---

## 📌 Overview

This project leverages **OpenCV**, **MediaPipe**, **YOLOv3**, and **Streamlit** to provide a multi-functional video analytics platform. The goal is to detect and visualize human actions and presence with minimal setup and intuitive user experience.

---

## 🧰 Features

| Module              | Description                                                             |
|---------------------|-------------------------------------------------------------------------|
| **Main Page**        | Landing page with Lottie animations and project description             |
| **Webcam Feed**      | View live video stream from your device                                 |
| **Object Detection** | Detects objects using YOLOv3 and draws bounding boxes                   |
| **Pose Detection**   | Uses TensorFlow pose models to render skeleton landmarks                |
| **Face Mesh**        | Applies MediaPipe face mesh model to live webcam input                  |
| **Intrusion Detection** | Alerts if a human body is detected in a camera frame                 |


## 🏗️ Project Structure

activity-detection-app/
│
├── Main.py # Main page with intro and animation
├── Feature.py # Webcam feed module
├── Object_Detection.py # YOLO-based object detection
├── Pose_Detection.py # Real-time pose tracking
├── Face_Mesh.py # Face mesh using MediaPipe
├── Intrusion_Detection.py # Human presence alert system
├── yolo/ # Contains YOLOv3 weights, cfg, and coco.names
│ ├── yolov3.weights
│ ├── yolov3.cfg
│ └── coco.names
├── requirements.txt
└── README.md

---

## ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/activity-detection-app.git
cd activity-detection-app
```

### 2. Install Dependencies
pip install -r requirements.txt

requirements.txt includes:

matplotlib==3.6.2
mediapipe==0.9.0
numpy==1.23.5
opencv_python==4.6.0.66
Pillow==9.3.0
requests==2.28.1
streamlit==1.15.1
streamlit_lottie==0.0.3


## 🚀 How to Run the App

streamlit run Main.py

Once the server starts, your default browser will open the app interface.


## 🧭 Navigation Instructions

1. Launch the app using the command above.
2. The Main Page shows animated introductions and project info.
3. Use the sidebar or navigation (depending on layout) to access:
    Webcam Feed: Live camera view.
    Object Detection: Detect real-world items.
    Pose Detection: See your body landmarks mapped.
    Face Mesh: Explore MediaPipe's advanced facial tracking.
    Intrusion Detection: Simulate security alert mechanisms.


## 💡 Notes

1. Ensure your system has a working webcam.
2. Place all YOLO model files inside the yolo/ directory as shown.
3. If facing performance issues, lower webcam resolution or frame rate.


## 🏁 Future Enhancements
1. Add face recognition and person tracking
2. Integrate email or SMS alerts for intrusion detection
3. Support cloud-based video storage
4. Deploy using Streamlit Cloud or Docker
