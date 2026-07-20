# YURA_ICMS_SYSTEM

## Overview

This repository serves as the **central repository** for the **YURA ICMS (In-Cabin Monitoring System)** project.

Since the project consists of multiple AI models with independent development cycles, each model is maintained in a separate Git repository.

This repository acts as an index that provides an overview of each model, its purpose, related repositories, and datasets.

---

# Model List

## 1. Object Detection

### Purpose
Detect objects inside the vehicle cabin to support OMS (Occupant Monitoring System) features.

Main features:
- Occupancy Detection
- Seatbelt Detection
- Child Presence Detection (CPD)
- Pet Detection
- Phone Detection
- Hands-on Detection (HOD)

### Repository
- Model Development
  - https://github.com/DeltaX-AI-Lab/icms-yolox

---

## 2. 2D Facial Landmark

### Purpose
Estimate facial landmarks for driver monitoring and facial analysis.

Main features:
- Driver Drowsiness Detection
- Driver Distraction Detection
- Eye Openness Estimation
- Facial Analysis

### Repository
- Model Development
  - https://github.com/DeltaX-AI-Lab/icms-face-landmark

---

## 3. Body Keypoint

### Purpose
Estimate occupant body keypoints for posture analysis and occupant monitoring.

Main features:
- Out-of-Position Detection
- Driver Behavior

### Repository

#### 3D Body Keypoint
- https://github.com/DeltaX-AI-Lab/icms-3d-body-metrabs

#### 2D Body Keypoint
- https://github.com/DeltaX-AI-Lab/mobis-oms-pose-estimation-yolox

---

## 4. Driver Behavior Classification

### Purpose
Classify driver behaviors to detect potentially unsafe driving actions.

Main features:
- Calling
- Drinking
- Eating
- Smoking
- Other

### Repository
- https://github.com/DeltaX-AI-Lab/icms-driver-behavior-classification

---

## 5. Head Pose Estimation

### Purpose
Estimate the driver's head orientation to support driver distraction detection.

Main features:
- Driver Distraction Detection

### Repository
- https://github.com/DeltaX-AI-Lab/3D_Gaze_Ground_Truth

---

## 6. Gaze Estimation

### Purpose
Estimate the driver's gaze direction for driver attention and distraction monitoring.

Main features:
- Driver Distraction Detection

### Repository
- https://github.com/DeltaX-AI-Lab/3D_Gaze_Ground_Truth

### Dataset
- GT Lab Gaze Dataset

---

## 7. Dynamic ROI (Auto Calibration)

### Purpose
Automatically adjust the Region of Interest (ROI) according to camera position or vehicle model, minimizing manual calibration.

### Repository
- https://github.com/DeltaX-AI-Lab/icms-dynamicROI
