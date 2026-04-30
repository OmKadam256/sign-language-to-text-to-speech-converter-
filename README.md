SilentEcho

AI-Based Real-Time Sign Language Recognition & Speech Converter

Python OpenCV MediaPipe Flask Machine Learning YOLO

📑 Table of Contents
📍 Problem Statement
📖 About the Project
✨ Key Features
🏗️ System Architecture
🛠️ Software Requirements
🚀 Technology Stack
📂 Dataset
📄 Research Paper
📘 Project Report
📊 Results & Accuracy
🔮 Future Scope
🏁 Getting Started
📍 Problem Statement

Communication between hearing-impaired individuals and the general public is challenging due to the lack of real-time translation systems. Most existing solutions are expensive, require specialized hardware, or fail to provide real-time performance.

SilentEcho addresses these challenges by developing a low-cost, real-time AI-based system that converts sign language gestures into text and speech using only a webcam.

📖 About the Project

SilentEcho is an AI/ML-based assistive communication system that enables users to translate hand gestures into meaningful text and speech in real-time.

The system integrates:

Computer Vision for hand tracking
Machine Learning for gesture classification
Text-to-Speech for voice output

This provides a seamless bridge between sign language users and non-sign language users.

✨ Key Features
✋ Gesture Recognition (Core Feature)
Detects 21 hand landmarks using MediaPipe
Supports:
Single-hand gestures (ASL)
Two-hand gestures (ISL)
Real-time gesture tracking using webcam
🧠 Machine Learning Model
Uses Random Forest Classifier
Lightweight and fast prediction
Trained on custom dataset
🔊 Speech Conversion
Converts recognized gestures into speech
Uses pyttsx3 (offline TTS engine)
🧩 Sentence Builder
Combine gestures into words
Build full sentences in real-time
🔐 Authentication System
User login & registration
SQLite-based backend
🤖 Hybrid AI System
MediaPipe → Fast detection
YOLO → Advanced classification
Auto mode switching
🏗️ System Architecture

SilentEcho follows a computer vision-based pipeline architecture integrating real-time gesture capture, feature extraction, and ML-based prediction.

Architecture Flow
graph TD
User --> Camera
Camera --> MediaPipe
MediaPipe --> LandmarkExtraction
LandmarkExtraction --> Normalization
Normalization --> ML_Model
ML_Model --> Prediction
Prediction --> Text
Prediction --> Speech
Text --> UI
Speech --> UI
🛠️ Software Requirements
🔹 Frontend
HTML
CSS
JavaScript
Flask Templates
🔹 Backend
Python
Flask
🔹 Libraries
OpenCV
MediaPipe
scikit-learn
pyttsx3
Ultralytics YOLO
🔹 Database
SQLite
🚀 Technology Stack
👁️ Computer Vision
OpenCV
MediaPipe
🧠 Machine Learning
Random Forest Classifier
YOLO Model
🌐 Backend
Flask
🎤 Speech
pyttsx3
💻 Frontend
HTML, CSS, JavaScript
📂 Dataset
🔗 Dataset Link

👉 https://drive.google.com/drive/folders/1p5wb8zP2BgJGclSVjybMAJz1KimUX9Zf

📊 Dataset Description
Custom dataset created using webcam
Each gesture recorded multiple times
Stored in CSV format

Each sample contains:

21 hand landmarks
X and Y coordinates
👉 Total = 42 features per sample
🧠 Dataset Usage
Dataset used to train Random Forest model
Split into:
80% Training
20% Testing
Used for real-time gesture prediction
📄 Research Paper
Title: SilentEcho: Real-Time Sign Language Recognition
Conference: IEEE ICCUBEA 2026
Contribution:
Real-time ML-based system
Low-cost assistive technology
Hybrid AI approach
📘 Project Report
Developed at FCRIT Vashi
Uses MediaPipe + Random Forest
Converts gestures → text → speech
📊 Results & Accuracy
ASL Accuracy: 94% – 96%
ISL Accuracy: 92% – 95%
Latency: < 50 ms (real-time)

👉 Based on experimental results

🔮 Future Scope
Deep Learning models (CNN, LSTM)
Mobile application
Multi-language support
Cloud deployment
Continuous gesture recognition
🏁 Getting Started
Prerequisites
Python 3.8+
Webcam
Run Locally
git clone https://github.com/your-username/SilentEcho.git
cd SilentEcho
pip install opencv-python mediapipe scikit-learn flask pyttsx3 ultralytics
python app.py
👨‍💻 Team
Om Kadam
Mayuresh Desai
Erwin Samuel
Sanskar Gharal
💡 Viva Line (IMPORTANT)

We created a custom dataset using MediaPipe hand landmarks and trained a Random Forest model to achieve real-time gesture recognition with high accuracy.

🔥 This is now:
