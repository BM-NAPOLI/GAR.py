# 📌 Face Recognition Attendance System (Arduino + Python + Flask)
**School:** El Gardgarat  
**Contributors:** BM-NAPOLI / Ahmed / IZAQ / Ostad  

A smart classroom attendance system using **a camera + AI** to detect and recognize faces, automatically mark attendance, and trigger an alert when an **unknown person** is detected. All activity is displayed in a **Web App dashboard**.

---

## 🧠 Project Idea

The system works like this:
- 📸 Captures faces using a USB webcam  
- ✅ Recognizes known students and marks attendance automatically  
- 🚨 If an unknown face appears, it triggers an alert (LED + Buzzer)  
- 🌐 Attendance and unknown detections are shown in a Flask Web App  

---

## 🎯 Objectives

- Reduce attendance cheating  
- Automate attendance recording  
- Improve classroom security by detecting unknown individuals  
- Combine **Arduino + Python + Web App** in one practical project  

---

## 🧩 Components

### 🔧 Hardware
- Arduino Uno / Nano  
- USB Webcam  
- LED  
- Buzzer  
- PC / Laptop  
- USB Cable  

### 💻 Software
- Python 3.10+  
- Arduino IDE  
- Flask  
- OpenCV  
- face-recognition  
- pyserial  
- SQLite (optional but recommended)  

---

## 🧠 Role Distribution

### 🧠 Python (The Brain)
- Start webcam and process frames  
- Face Detection  
- Face Recognition  
- Attendance logging (CSV / DB)  
- Send commands to Arduino via Serial (USB)  
- Communicate with Flask Web App  

### 🤖 Arduino (The Executor)
- Control LED  
- Control Buzzer  
- Receive commands from Python only  

### 🌐 Web App (Flask)
- Display attendance table  
- Display unknown faces with timestamps  
- Teacher dashboard + student management  

---

---

## 🌐 Web App Pages

### 1) Login (Optional)
- Teacher authentication  

### 2) Dashboard
- Total present  
- Total absent  
- Total unknown faces detected  

### 3) Attendance Page
| Name | Time | Status |

### 4) Unknown Faces
- Image of unknown person  
- Timestamp  
- Actions: Add as student / Ignore  

### 5) Students Management
- Add student  
- Upload student photo  
- Remove student  

---

## 🗂️ Project Structure


---

## 🎬 Workflow Scenario

1. Start the system  
2. Someone enters the classroom  
3. Webcam captures a frame  
4. Python detects and compares the face  
5. If known → mark attendance  
6. If unknown → trigger Arduino alert + save snapshot + show in Web App  

---

## 📚 Required Knowledge

- Python basics  
- OpenCV fundamentals  
- Face recognition (face-recognition library)  
- Arduino basics  
- Serial communication (pyserial)  
- Flask basics (routes, templates, database)  

---

## 🪜 Roadmap

### Phase 1 — Detection Only
- Webcam working  
- Detect faces (no recognition)  

### Phase 2 — Recognition + Logging
- Encode known faces  
- Recognize faces  
- Save attendance (CSV/DB)  

### Phase 3 — Arduino Integration
- Serial connection Python ↔ Arduino  
- LED/Buzzer alerts for unknown faces  

### Phase 4 — Web App
- Dashboard UI  
- Attendance view  
- Unknown faces management  
- Student management  

---

## ✅ Important Notes

- Face recognition does **NOT** run on Arduino.  
- Arduino only executes commands (LED/Buzzer).  
- Python is the core of the system.  
- Web App works on any device connected to the same network (if hosted properly).  

---

## 🚀 Future Improvements (Optional)

- Add admin roles / multi-teacher support  
- Use a real database with sessions and reports  
- Export attendance as PDF/Excel  
- Add anti-spoofing (photo/video attack detection)  

---

.. RAYAN MINAZZOU ..

## 🏗️ System Architecture

