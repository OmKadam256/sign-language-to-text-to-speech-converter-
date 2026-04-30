<p align="center"> <strong>AI-Based Real-Time Sign Language Recognition & Speech Conversion System</strong> </p> <p align="center"> <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/OpenCV-Computer_Vision-green?style=for-the-badge&logo=opencv" /> <img src="https://img.shields.io/badge/MediaPipe-Hand_Tracking-orange?style=for-the-badge" /> <img src="https://img.shields.io/badge/Flask-Web_App-black?style=for-the-badge&logo=flask" /> <img src="https://img.shields.io/badge/Machine_Learning-RandomForest-red?style=for-the-badge" /> </p>
🚀 Overview

SilentEcho is an AI-powered assistive communication system that translates sign language gestures into text and speech in real time using computer vision and machine learning.

👉 Designed to help deaf and mute individuals communicate effectively using just a webcam.

📑 Table of Contents
📍 Problem Statement
📖 About the Project
✨ Features
🏗️ System Architecture
⚙️ Working Methodology
📂 Dataset
📄 Research Paper
📘 Project Report
📊 Results & Accuracy
🛠️ Tech Stack
🧪 Installation
🚀 Future Scope
👨‍💻 Team
📍 Problem Statement

Communication between hearing-impaired individuals and others is difficult due to lack of real-time translation tools.

❌ Existing systems:

Expensive (sensor gloves, Kinect)
Not portable
Not real-time

✅ Solution: SilentEcho

Low-cost
Real-time
Works with normal webcam
📖 About the Project

SilentEcho uses MediaPipe + Machine Learning to detect hand gestures and convert them into:

✔ Text
✔ Speech
✔ Sentences

👉 It runs completely offline on standard hardware.

✨ Key Features
✋ Real-Time Gesture Recognition
Detects 21 hand landmarks
Works with single-hand (ASL) and dual-hand (ISL)
🧠 AI-Based Prediction
Random Forest Classifier
Fast & lightweight
🔊 Speech Conversion
Converts text → speech using pyttsx3
🔤 Multi-Language Support
ASL (American Sign Language)
ISL (Indian Sign Language)
🧩 Sentence Builder
Combine gestures into words
Real-time sentence creation
🔐 Authentication System
Login/Register using Flask + SQLite
🤖 Hybrid AI System
MediaPipe (fast)
YOLO (advanced detection)
🏗️ System Architecture
⚙️ Working Methodology

1️⃣ Webcam captures hand gesture
2️⃣ MediaPipe extracts 21 landmarks
3️⃣ Data normalized (relative coordinates)
4️⃣ Random Forest predicts gesture
5️⃣ Output displayed as text
6️⃣ Converted into speech

📂 Dataset Usage in Project
📊 Custom Dataset Creation

This project uses a self-collected dataset created using a webcam instead of relying on pre-built datasets.

👉 Dataset Link:
https://drive.google.com/drive/folders/1p5wb8zP2BgJGclSVjybMAJz1KimUX9Zf

🧪 How Dataset Was Created
Open the data collection script
Enter the gesture label (e.g., A, B, Hello)
Show hand gesture in front of camera
System captures multiple samples per gesture
Data stored in CSV file

✔ Each sample contains:

21 hand landmarks
X and Y coordinates
Total = 42 features per sample
⚙️ Data Processing
Landmark points are extracted using MediaPipe
Data is normalized relative to wrist position
This ensures:
Position independence
Better model accuracy
🧠 How Dataset is Used
1️⃣ Training Phase
Dataset loaded from CSV file
Features (X, Y coordinates) extracted
Labels assigned (gesture names)
Model used:
👉 Random Forest Classifier
Dataset split:
Training: 80%
Testing: 20%
2️⃣ Model Learning
Model learns patterns of hand landmarks
Identifies differences between gestures
Builds decision trees for classification
3️⃣ Real-Time Prediction
Live camera captures gesture
Landmarks extracted
Compared with trained dataset
Model predicts gesture instantly
📄 Research Paper

📌 Title: SilentEcho: Real-Time Sign Language Recognition

📌 Conference:
IEEE ICCUBEA 2026 (Pune)

📌 Contribution:

Real-time gesture recognition
Low-cost AI system
Hybrid approach (MediaPipe + YOLO)
📘 Project Report

📄 Mini Project Report:
👉 Upload PDF in repo and add link here

📌 Highlights:

Developed at FCRIT Vashi
Uses MediaPipe + Random Forest
Converts gestures into speech
📊 Results & Accuracy
🎯 ASL Accuracy: 94% – 96%
🎯 ISL Accuracy: 92% – 95%
⚡ Latency: < 50 ms (real-time)
🛠️ Tech Stack
👁️ Computer Vision
OpenCV
MediaPipe
🧠 Machine Learning
Random Forest
YOLO
🌐 Backend
Flask
SQLite
🎤 Speech
pyttsx3
💻 Frontend
HTML
CSS
JavaScript
🧪 Installation
git clone https://github.com/your-username/SilentEcho.git
cd SilentEcho
pip install opencv-python mediapipe scikit-learn flask pyttsx3 ultralytics
python app.py
📸 Screenshots (Add for Best Impact)
/images/demo1.png  
/images/demo2.png  
/images/ui.png  
🎥 Demo Video (Optional but Powerful)

Add YouTube / Drive link here

🚀 Future Scope
Deep Learning (CNN, LSTM)
Mobile App (Android/iOS)
Multi-language speech
Cloud-based system
Continuous gesture recognition
