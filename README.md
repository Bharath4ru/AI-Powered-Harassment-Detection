# README: Sexual Harassment Detection and Safety Monitoring System

## Inspiration  
<img src="https://user-images.githubusercontent.com/130077430/230579469-c1263cef-784e-4845-93fb-2f73544e49e1.png" width="90" height="80">
Throughout our lives, we've been exposed to countless reports and stories in newspapers and online platforms, underscoring the distressing prevalence of sexual harassment incidents. The reluctance victims often experience when reporting such incidents due to fears of retaliation or social stigma drove the creation of this project. The aim is to leverage innovative technologies to create a safer, more inclusive work environment.

## Problem Statement
<img src="https://user-images.githubusercontent.com/130077430/230730194-a7389fed-f5fd-48d3-856a-0212057f2500.png" width="90" height="80">
The goal is to build a technological solution for real-time harassment detection while addressing the gaps left by traditional methods. This includes creating a safer work environment, overcoming reporting hesitancy, supporting HR and legal management, reducing stress, and ensuring early detection and prevention of harassment.

---

# Introduction
<img src="https://user-images.githubusercontent.com/72274851/152814876-73362bcc-bde6-411f-ba80-235e911f276f.gif" width="90" height="90">
The project aims to develop a CNN-based model to detect workplace harassment and a **Safety Monitoring System with Email Alert and Face Recognition** module. This hybrid approach ensures accurate detection of harassment behavior while enhancing workplace safety through real-time face recognition and alert notifications.

---

# Modules Overview

### 1. **Harassment Detection System**
This module leverages a CNN-based model to differentiate harassment behaviors from normal workplace activities in videos.

### 2. **Safety Monitoring System with Email Alerts and Face Recognition**
A real-time monitoring solution using facial recognition technology integrated with safety protocols.
- **Features:**
  - Face recognition to identify individuals in the workplace.
  - Real-time monitoring to detect anomalies.
  - Instant email alerts sent to security and management in case of unauthorized access or suspicious behavior.

---

# Approach
<img src="https://cdn0.iconfinder.com/data/icons/data-science-2-1/66/119-512.png" width="90" height="80">

### Harassment Detection System
- **Model:** CNN with transfer learning (VGG16, Xception).
- **Dataset:** Custom dataset with 1,000 harassment and 1,000 non-harassment images.
- **Data Split:** 80% training, 20% testing.

### Safety Monitoring System
- **Face Recognition:** Utilizes OpenCV and dlib for detecting faces and matching against a pre-registered database.
- **Email Alerts:** Python's SMTP library sends notifications upon detecting unauthorized individuals or safety concerns.
- **Data Sources:** Pre-trained models and a custom facial dataset collected for workplace safety monitoring.

---

# Procedure
<img src="https://th.bing.com/th/id/R.02832177b40b49d50674126476f980c3?rik=aXibwvpQe645bg&riu=http%3a%2f%2fwww.clipartbest.com%2fcliparts%2fjcx%2f6rb%2fjcx6rbngi.png&ehk=xllVkMLnEE%2fEXx%2fnWbpceiVVfvTNGJmODcZ9fEBJVGA%3d&risl=&pid=ImgRaw&r=0" width="120" height="100">

## 1. Pre-Installation
Install the following libraries:
- OpenCV
- Keras
- TensorFlow
- dlib
- Pandas
- NumPy
- OS
- SMTP (for email alerts)

## 2. Dataset Preparation
- **Harassment Detection:**
  - 2 folders: `yes` (harassment images) and `no` (healthy environment images).
  - Images resized to 224x224x3.
  - Converted into NumPy arrays and split into training/testing sets.

- **Face Recognition:**
  - A database of employee faces is pre-registered.
  - Images are preprocessed for facial encoding using dlib’s facial recognition model.

## 3. Model Training
- **Harassment Detection:**
  - CNN model using VGG16 architecture.
  - Optimized using Intel OneAPI for better performance.

- **Safety Monitoring System:**
  - Face encoding matching using cosine similarity.
  - Real-time monitoring using OpenCV for video feed integration.

## 4. Deployment
- **Application:**
  - Flutter-based app integrates both modules.
  - Alerts are displayed on the app with real-time notifications.
  - Admin access to employee records and system logs.

---

# Results

### Harassment Detection
Achieved 98% training accuracy and 97% validation accuracy.

### Safety Monitoring
- Recognized faces with 95% accuracy in real-time.
- Instant email alerts successfully sent for all test cases.

---

# Learnings

1. **Machine Learning:**
   - Developed expertise in training CNN models for video analysis.
   - Implemented transfer learning to improve detection accuracy.

2. **Face Recognition:**
   - Used dlib and OpenCV for robust facial recognition.
   - Integrated real-time recognition with anomaly detection.

3. **Deployment:**
   - Built a cross-platform Flutter app for user interaction and notifications.

4. **Optimization:**
   - Leveraged Intel OneAPI to optimize model performance on heterogeneous systems.

---

# Future Enhancements
1. Expand the facial recognition database for scalability.
2. Integrate emotion recognition to identify stress or discomfort.
3. Enable voice alerts in addition to email notifications.
4. Explore IoT integration for enhanced real-time monitoring.

---

# Conclusion
By combining **Harassment Detection** with a **Safety Monitoring System**, this project addresses workplace safety comprehensively. It fosters a secure environment, supports HR processes, and promotes early intervention for safety and harassment concerns.
