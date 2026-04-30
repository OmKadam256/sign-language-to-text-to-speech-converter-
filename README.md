🧠 SilentEcho
<p align="center"> <strong>AI-Based Real-Time Sign Language Recognition & Speech Conversion System</strong> </p> <p align="center"> <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/OpenCV-Computer_Vision-green?style=for-the-badge&logo=opencv" /> <img src="https://img.shields.io/badge/MediaPipe-Hand_Tracking-orange?style=for-the-badge" /> <img src="https://img.shields.io/badge/Flask-Web_App-black?style=for-the-badge&logo=flask" /> <img src="https://img.shields.io/badge/Machine_Learning-RandomForest-red?style=for-the-badge" /> </p>
🚀 Overview

SilentEcho is an AI-powered assistive communication system that converts sign language gestures into text and speech in real time using computer vision and machine learning.

👉 Designed to help deaf and mute individuals communicate effectively using a webcam.

📍 Problem Statement

Communication barriers exist because most people do not understand sign language.

❌ Existing systems:

Expensive hardware
Not portable
Slow processing

✅ Solution: SilentEcho

Low-cost
Real-time
Runs on normal laptops
📖 About the Project

SilentEcho uses MediaPipe + Machine Learning to detect hand gestures and convert them into:

✔ Text
✔ Speech
✔ Sentences

👉 Works completely offline on standard hardware.

✨ Key Features
✋ Real-time gesture recognition
🔤 ASL + 🇮🇳 ISL support
🔊 Text-to-Speech conversion
🧠 Random Forest ML model
🧩 Sentence formation system
🔐 Login & authentication system
🤖 Hybrid AI (MediaPipe + YOLO)
🏗️ System Architecture
⚙️ Working Methodology
Webcam captures gesture
MediaPipe extracts 21 landmarks
Data normalized
Random Forest predicts gesture
Output displayed as text
Converted into speech
📂 Dataset (IMPORTANT)
🔗 Dataset Link

👉 https://drive.google.com/drive/folders/1p5wb8zP2BgJGclSVjybMAJz1KimUX9Zf

🧪 How Dataset is Created
Custom dataset created using webcam
Each gesture recorded multiple times
Stored in CSV format

Each sample contains:

21 hand landmarks
X and Y coordinates
Total = 42 features
🧠 How Dataset is Used
🔹 Training Phase
Dataset loaded from CSV
Features extracted
Labels assigned
Model trained using Random Forest
🔹 Testing Phase
Dataset split (80% train / 20% test)
🔹 Prediction Phase
Live gesture captured
Compared with trained dataset
Model predicts output in real-time
🔁 Dataset Workflow
📄 Research Paper

📌 Title: SilentEcho: Real-Time Sign Language Recognition

📌 Conference Submission:
IEEE ICCUBEA 2026

📌 Contribution:

Real-time ML system
Low-cost assistive technology
Hybrid AI approach
📘 Project Report

📄 Based on your actual report:

Developed at FCRIT Vashi
Uses MediaPipe + Random Forest
Converts gestures → text → speech

📌 Abstract Summary:

The system uses MediaPipe for landmark detection and Random Forest for classification to achieve real-time gesture recognition with high accuracy.

📊 Results & Accuracy
🎯 ASL Accuracy: 94% – 96%
🎯 ISL Accuracy: 92% – 95%
⚡ Latency: < 50 ms

👉 Verified in project report

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
HTML, CSS, JavaScript
🧪 Installation
git clone https://github.com/your-username/SilentEcho.git
cd SilentEcho
pip install opencv-python mediapipe scikit-learn flask pyttsx3 ultralytics
python app.py
📸 Screenshots (Add Images for More Marks)
/images/demo1.png
/images/ui.png
/images/output.png
🎥 Demo Video

(Add YouTube / Drive link here)

🚀 Future Scope
Deep learning (CNN, LSTM)
Mobile app
Multi-language support
Cloud deployment
Continuous gesture recognition
