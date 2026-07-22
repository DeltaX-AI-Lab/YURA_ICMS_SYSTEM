# YURA_ICMS_SYSTEM

## Overview

This repository serves as the **central repository** for the **YURA ICMS (In-Cabin Monitoring System)** project.

Since the project consists of multiple AI models with independent development cycles, each model is maintained in a separate Git repository.

This repository acts as an index that provides an overview of each model, its purpose and related repositories.

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
 
### version
| Version| Name  | dataset | train by | Note | origin |
|-------|---------|-----|-------|------|----|
| v1.0|object-detection_v1.0| | sami | add child class | detection_20260630_v6 |


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

### version
| Version| Name | dataset | train by | Note | path |
|-------|---------|-----|-------|------|----|
| v1.0|face-detection_v1.0| | binh | Train with new data | facial_20260227_v2/model/20251120.onnx |

---

## 3. 3D Body Keypoint

### Purpose
Estimate occupant body keypoints for posture analysis and occupant monitoring.

Main features:
- Out-of-Position Detection
- Driver Behavior

### Repository

#### 3D Body Keypoint
- https://github.com/DeltaX-AI-Lab/icms-3d-body-metrabs

### version
| Version| Name | dataset | train by | Note | path |
|-------|---------|-----|-------|------|----|
| v1.0|3d-body-keypoint_v1.0 | | yunho | merge driver & front | body_3d/body_3d_20260318_v2/model/eff2s_coco19_backbone_head.onnx |

---

## 4. 2D Body Keypoint

### Purpose
Estimate occupant body keypoints for posture analysis and occupant monitoring.

Main features:
- Out-of-Position Detection
- Driver Behavior

### Repository
#### 2D Body Keypoint
- https://github.com/DeltaX-AI-Lab/mobis-oms-pose-estimation-yolox

### version
| Version| Name |dataset | train by | Note | path |
|-------|---------|-----|-------|------|----|
| v1.0|3d-body-keypoint_v1.0 | | binh | PHA Final | body_kpts/body_kpts_20260227_v2/model/body_keypoints_0303.onnx |

---

## 5. Driver Behavior Classification

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

### version
| Version| Name | dataset | train by | Note | path |
|-------|---------|-----|-------|------|----|
| v1.0|behavior_v1.0 | binh | accuracy improved + size reduced | driver_behaviour_20260518_v2/model/PHA_Driver_Behavior_dev_mobilenet_v2_V6.0_350x350.onnx |

---

## 6. Gaze Estimation

### Purpose
Estimate the driver's gaze direction for driver attention and distraction monitoring.

Main features:
- Driver Distraction Detection

### Repository
- https://github.com/DeltaX-AI-Lab/3D_Gaze_Ground_Truth

### version
| Version| Name | dataset | train by | Note | path |
|-------|---------|-----|-------|------|----|
| v1.0|gaze_v1.0 | | maksym | accuracy improved + input size changed | gaze_20260514_v4_qat_v1/model/best_model_qat.onnx |



---

## 7. Head Pose Estimation
### Purpose
Estimate the driver's head orientation to support driver distraction detection.

Main features:
- Driver Distraction Detection

### Repository
- https://github.com/DeltaX-AI-Lab/3D_Gaze_Ground_Truth

---

## 8. Dynamic ROI (Auto Calibration)

### Purpose
Automatically adjust the Region of Interest (ROI) according to camera position or vehicle model, minimizing manual calibration.

### Repository
- https://github.com/DeltaX-AI-Lab/icms-dynamicROI
