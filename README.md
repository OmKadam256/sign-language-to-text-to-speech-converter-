🧠 SilentEcho
<p align="center"> <strong>AI-Based Real-Time Sign Language Recognition & Speech Conversion System</strong> </p> <p align="center"> <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python" /> <img src="https://img.shields.io/badge/OpenCV-Computer_Vision-green?style=for-the-badge&logo=opencv" /> <img src="https://img.shields.io/badge/MediaPipe-Hand_Tracking-orange?style=for-the-badge" /> <img src="https://img.shields.io/badge/Flask-Web_App-black?style=for-the-badge&logo=flask" /> <img src="https://img.shields.io/badge/Machine_Learning-RandomForest-red?style=for-the-badge" /> </p>
🚀 Overview

SilentEcho is an AI-powered assistive communication system that translates sign language gestures into text and speech in real-time.

👉 It uses Computer Vision + Machine Learning and works using a simple webcam — no expensive hardware required.

📍 Problem Statement

Communication between hearing-impaired individuals and others is difficult because most people do not understand sign language.

❌ Existing Problems:
Expensive hardware (Kinect, sensor gloves)
Not portable
Not real-time
Requires internet
✅ Proposed Solution:

SilentEcho provides:

Real-time recognition
Low-cost solution
Offline working
Easy usability
📖 About the Project

SilentEcho detects hand gestures and converts them into:

✔ Text
✔ Speech
✔ Sentences

👉 Built using:

MediaPipe (hand tracking)
Random Forest (ML model)
Flask (web interface)
✨ Key Features
✋ Gesture Recognition
Detects 21 hand landmarks
Supports:
Single hand (ASL)
Two hands (ISL)
🧠 Machine Learning
Random Forest Classifier
Fast + lightweight
🔊 Speech Output
Text → Speech using pyttsx3
🔤 Multi Language Support
ASL (American Sign Language)
ISL (Indian Sign Language)
🧩 Sentence Builder
Combine gestures into words
Real-time sentence formation
🔐 Authentication
Login/Register system
🤖 Hybrid AI
MediaPipe (fast)
YOLO (advanced)
🏗️ System Architecture
graph TD
User --> Camera
Camera --> MediaPipe
MediaPipe --> LandmarkExtraction
LandmarkExtraction --> Normalization
Normalization --> MLModel
MLModel --> Prediction
Prediction --> Text
Prediction --> Speech
Text --> UI
Speech --> UI
⚙️ Working Methodology
Step 1: Input

Webcam captures hand gesture

Step 2: Detection

MediaPipe extracts 21 landmarks

Step 3: Processing

Landmarks normalized (relative to wrist)

Step 4: Prediction

Random Forest model predicts gesture

Step 5: Output
Text displayed
Converted to speech
📂 Dataset (VERY IMPORTANT)
🔗 Dataset Link

👉 https://drive.google.com/drive/folders/1p5wb8zP2BgJGclSVjybMAJz1KimUX9Zf

🧪 Dataset Creation

We created our own dataset using webcam:

Run data collection script
Enter gesture label
Show gesture
System records multiple samples
Stored in CSV
📊 Dataset Structure

Each row contains:

Label (gesture name)
21 landmark X values
21 landmark Y values

👉 Total = 42 features per sample

🧠 How Dataset is Used
🔹 Training
Dataset loaded from CSV
Features extracted
Labels assigned
Model trained (Random Forest)
🔹 Testing
Split:
80% training
20% testing
🔹 Prediction
Live gesture captured
Compared with trained data
Output predicted in real-time
🔁 Dataset Workflow
graph TD
A[Capture Gesture] --> B[Store CSV]
B --> C[Normalize Data]
C --> D[Train Model]
D --> E[Real-Time Prediction]
📄 Research Paper

📌 Title:
SilentEcho: Real-Time Sign Language Recognition

📌 Conference:
IEEE ICCUBEA 2026

📌 Contribution:

Real-time ML system
Low-cost communication tool
Hybrid AI model
📘 Project Report

📄 Based on your official submission:

👉

📌 Highlights:
Developed at FCRIT Vashi
Uses MediaPipe + Random Forest
Converts gestures → text → speech
📌 Abstract:

The system uses MediaPipe for hand landmark detection and Random Forest classifier to recognize gestures in real-time and convert them into text and speech.

📊 Results & Accuracy

From your report:

🎯 ASL Accuracy: 94% – 96%
🎯 ISL Accuracy: 92% – 95%
⚡ Latency: < 50 ms

👉 Verified in Chapter 5 of report

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
📸 Screenshots

(Add these images in your repo for best marks)

/images/demo1.png  
/images/ui.png  
/images/output.png  
🎥 Demo Video

(Add YouTube / Drive link here)

🚀 Future Scope
Deep Learning (CNN, LSTM)
Mobile App
Multi-language speech
Cloud integration
Continuous gesture recognition
👨‍💻 Team
Om Kadam
Mayuresh Desai
Erwin Samuel
Sanskar Gharal
