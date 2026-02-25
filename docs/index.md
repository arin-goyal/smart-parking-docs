---
layout: default
title: Home
---

# 🚗 Smart Parking Detection System

### Classical Computer Vision Project

---

📍 **Course:** Computer Vision  
📍 **Type:** Academic Project Proposal  
📍 **Approach:** Classical CV (No Deep Learning)

---

---

## 📌 Problem Statement

In large multi-level parking facilities such as malls, airports, and universities, drivers often spend significant time searching for available parking spaces. This results in increased traffic congestion, fuel wastage, and inefficient utilization of parking infrastructure.

Existing systems rely on either sensor-based solutions, which are costly and require additional hardware, or deep learning-based systems that demand high computational resources.

There is a need for a cost-effective, scalable, and efficient solution that can utilize existing infrastructure.

---

## 🎯 Proposed Solution

We propose a smart parking detection system that uses classical computer vision techniques to analyze CCTV video feeds and determine the occupancy status of parking slots in real time.

The system identifies parking slots and classifies them as:

- 🟢 Empty  
- 🔴 Occupied  

The solution is lightweight, explainable, and does not rely on deep learning.

---

## ⭐ Objectives

### Primary Objective

To design a real-time parking slot detection system using classical computer vision techniques.

### Specific Objectives

- To preprocess video frames for improved clarity  
- To detect foreground objects using background subtraction  
- To define parking slots using region-based annotation  
- To classify each parking slot as occupied or vacant  
- To visualize results in real time  

---

## 🏢 Existing Solutions

### Sensor-Based Systems

- Require hardware installation per slot  
- High cost and maintenance  
- Not scalable for existing infrastructure  

### Deep Learning Systems

- Require GPU and large datasets  
- Computationally expensive  
- Black-box models with low interpretability  

---

## 🚀 What Makes Our System Unique

- Uses only classical computer vision  
- No additional hardware required  
- Works with existing CCTV cameras  
- Lightweight and real-time capable  
- Fully explainable pipeline  

---

## 🧠 Methodology

### 1. System Architecture & Tech Stack

- Language: Python  
- Libraries: OpenCV, NumPy  
- Input: CCTV video feed  
- Output: Real-time occupancy visualization  

---

### 2. Module Development (Input)

#### Video Preprocessing
- Convert frames to grayscale  
- Apply CLAHE for contrast enhancement  
- Apply Gaussian blur for noise reduction  

#### Foreground Detection
- Apply background subtraction (MOG2)  
- Identify moving objects  

#### Slot Annotation
- Manually define parking slots  
- Represent each slot as a polygon (ROI)  

---

### 3. Execution & Integration (Process)

- Capture video frames  
- Apply preprocessing  
- Perform foreground detection  
- Load parking slot coordinates  
- For each slot:
  - Create mask  
  - Compute pixel density  
  - Classify as occupied or empty  
- Display results  

---

### 4. Testing & Validation (Output)

- Accuracy of detection  
- Stability of classification  
- Frame processing speed (FPS)  
- Performance under different lighting conditions  

---

### 5. Constraints

- Sensitive to lighting conditions  
- Shadows may affect detection  
- Requires fixed camera position  
- Static object detection limitations  

---

## 🗂️ System Pipeline

```
Video Input → Preprocessing → Foreground Detection → Slot Detection → Occupancy Classification
```

---

## 📅 Timeline

| Week | Task |
|------|------|
| 1-2 | Problem definition and research |
| 3-4 | Preprocessing implementation |
| 5-6 | Background subtraction |
| 7-8 | Slot detection |
| 9-10 | Occupancy classification |
| 11-12 | Testing and refinement |

---

## 📦 Resources

- Python (OpenCV, NumPy)  
- CCTV video dataset  
- Personal computer  

No external funding required.

---

## 🔮 Future Scope

- Improve accuracy for static vehicles  
- Multi-camera integration  
- Nearest parking slot recommendation  
- Mobile/web interface  

---

## 📌 Conclusion

This project demonstrates that efficient parking detection can be achieved using classical computer vision techniques without relying on deep learning. The proposed system is cost-effective, scalable, and suitable for real-time deployment using existing infrastructure.

---