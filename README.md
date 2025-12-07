# 🧍‍♂️ Foot-Fall-Analysis  
### Intelligent People Counting & Foot-Traffic Analytics using Computer Vision

## 📌 **Project Overview**

Foot-Fall-Analysis is a Computer Vision–based Python project that detects, counts, and analyzes human foot traffic in real-time.  
It processes either **webcam feed** or **video input**, identifies people using detection models, and produces **real-time foot-fall counts**, optionally enriched with **age & gender analysis**.

This system is ideal for:

- Retail stores & malls  
- Queue monitoring  
- Crowd analytics  
- Smart surveillance  
- Visitor insights  

The project is built to be **modular**, **efficient**, and **easy to integrate** into larger systems.

---

## 🚀 **Features**

### ✔ Real-Time Foot-Fall Counting  
Detects humans live using video feed and tracks foot-fall across the frame.

### ✔ Model-Based Person Detection  
Efficient detection pipeline implemented in `Detection.py`.

### ✔ Optional Age & Gender Estimation  
Pre-trained age/gender models located inside `age_gender_model/`.

### ✔ Clean and Modular Codebase  
Utilities separated in `utils.py` and video handling in `Cam.py`.

### ✔ Video / Webcam Input  
Switch between real-time camera or video file with minimal changes.

### ✔ Easy to Customize  
You can:  
- change detection model  
- modify counting logic  
- integrate with databases  
- export analytics  

### **1️⃣ Clone the Repository**

git clone https://github.com/mansooriabu25/Foot-Fall-Analysis.git
cd Foot-Fall-Analysis

## 📁 **How To Run **
1. Create Virtual Environment (Recommended)
   python -m venv venv
   venv\Scripts\activate

2. Install Dependencies
   pip install -r requirements.txt

3. Run the Project
   python main.py


🎥 How It Works
📌 1. Capture Video Frames

Handled by Cam.py
Can read from webcam
Can read from video file

📌 2. Human Detection

Detection.py
Uses pre-trained detection models
Extracts bounding boxes for detected persons

📌 3. Age & Gender Prediction (Optional)

age_gender_model/ directory
Lightweight CNN model
Predicts age group & gender

📌 4. Foot-Fall Counting Logic

Implemented inside utils.py
Tracks person entering/exiting ROI
Maintains stable count
Avoids double-counting

📌 5. Real-Time Rendering

Bounding boxes
Tracking lines
Foot-fall counters
Optional age & gender overlays
