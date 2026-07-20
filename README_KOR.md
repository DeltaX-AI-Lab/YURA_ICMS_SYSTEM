# YURA_ICMS_SYSTEM

## Overview

이 Repository는 **YURA Project의 ICMS(In-Cabin Monitoring System)** 에 사용되는 AI 모델들을 관리하기 위한 중앙 Repository입니다.

프로젝트 규모가 크기 때문에 각 AI 모델은 독립적인 Repository에서 개발 및 관리됩니다.
본 Repository는 각 모델의 목적, 관련 Repository 등의 정보를 관리하는 Index 역할을 수행합니다.

---

# Model List

## 1. Object Detection

### Purpose
차량 내부의 객체를 검출하여 OMS 기능을 수행합니다.

주요 기능
- Occupancy Detection
- Seatbelt Detection
- Child Presence Detection (CPD)
- Pet Detection
- Phone Detection
- Hands On Detection(HOD)

### Repository
- Model Code
  - https://github.com/DeltaX-AI-Lab/icms-yolox

---

## 2. Facial Landmark (2D)

### Purpose
운전자 얼굴 Landmark를 검출하여 졸음 및 운전자 상태를 분석합니다.

주요 기능
- Driver Drowsiness
- Driver Distraction
- Eye Openness
- Facial Analysis

### Repository
- Model Code
  - https://github.com/DeltaX-AI-Lab/icms-face-landmark

---

## 3. Body Keypoint

### Purpose
탑승자의 신체 Keypoint를 추정하여 자세 및 위치를 분석합니다.

주요 기능
- Out of Position Detection
- Driver Behavior

### Repository

#### 3D Body Keypoint
- https://github.com/DeltaX-AI-Lab/icms-3d-body-metrabs

#### 2D Body Keypoint
- https://github.com/DeltaX-AI-Lab/mobis-oms-pose-estimation-yolox

---

## 4. Driver Behavior Classification

### Purpose
운전자의 행동을 분류하여 운전 중 위험 행동을 감지합니다.

주요 기능
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
운전자의 머리 방향을 추정하여 주의 분산 여부를 판단합니다.

주요 기능
- Driver Distraction

### Repository
- https://github.com/DeltaX-AI-Lab/3D_Gaze_Ground_Truth

---

## 6. Gaze Estimation

### Purpose
운전자의 시선을 추정하여 Driver Distraction 기능을 수행합니다.

주요 기능
- Driver Distraction

### Repository
- https://github.com/DeltaX-AI-Lab/3D_Gaze_Ground_Truth

---

## 7. Dynamic ROI (Auto Calibration)

### Purpose
차종 또는 카메라 위치 변경 시 ROI를 자동으로 설정하여 Calibration 작업을 최소화합니다.

### Repository
- https://github.com/DeltaX-AI-Lab/icms-dynamicROI
