# 🌌 Face Detection using Haar Cascades

## 📖 Overview
This project demonstrates **Face Detection** and **Eye Detection** using OpenCV Haar Cascade Classifiers.  
The system detects human faces and eyes in both images and real-time webcam video streams.

> ⚠️ Note: This project performs **Face Detection**, not Face Recognition.  
> It detects the presence of faces but does not identify who the person is.

---

## 🛠️ Technologies Used
- Python
- OpenCV
- NumPy
- Matplotlib

---

## 🎯 Features
✅ Face Detection in Images  
✅ Eye Detection in Images  
✅ Real-Time Webcam Face Detection  
✅ Haar Cascade Classifier Integration  
✅ Rectangle Highlighting for Detected Regions

---

## 📂 Project Workflow

### 1️⃣ Load and Display Images
- Imported required libraries
- Loaded grayscale images using `cv2.imread()`
- Displayed images using Matplotlib

### 2️⃣ Face Detection
- Loaded Haar Cascade face classifier
- Detected faces using `detectMultiScale()`
- Drew white rectangles around detected faces

### 3️⃣ Eye Detection
- Loaded Haar Cascade eye classifier
- Detected eyes inside images
- Highlighted eyes with white rectangles

### 4️⃣ Real-Time Webcam Detection
- Captured video using webcam
- Applied face detection on each frame
- Displayed live detection output
- Stopped video using keyboard interrupt

---

## 💻 Sample Code

```python
face_cascade = cv2.CascadeClassifier(
    cv2.data.haarcascades + 'haarcascade_frontalface_default.xml'
)

faces = face_cascade.detectMultiScale(
    img,
    scaleFactor=1.2,
    minNeighbors=5
)
```

---

## 📷 Applications
- Surveillance Systems
- Smart Attendance Systems
- Security Applications
- Human-Computer Interaction
- AI Vision Systems

---

## ✨ Conclusion
This project demonstrates the fundamentals of computer vision using Haar Cascade classifiers for detecting faces and eyes in images and real-time video streams.  
It serves as a beginner-friendly introduction to object detection using OpenCV.
