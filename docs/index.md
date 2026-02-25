# Smart Parking Detection using Classical Computer Vision

## 1. Introduction / Problem Statement

In large multi-level parking areas such as malls, airports, and universities, drivers often spend significant time searching for available parking spots. This leads to increased congestion, fuel consumption, and inefficient utilization of parking space.

Existing solutions either rely on sensor-based infrastructure, which is expensive and difficult to maintain, or deep learning-based systems, which require high computational resources and lack interpretability.

This project aims to develop a cost-effective and efficient parking detection system using classical computer vision techniques. By utilizing existing CCTV camera feeds, the system detects occupied and vacant parking slots in real time without requiring additional hardware or deep learning models.

---

## 2. Objectives

The primary objective of this project is to design and implement a real-time parking slot detection system using classical computer vision.

### Specific Objectives:

- To preprocess video frames for enhanced visibility and noise reduction  
- To detect foreground objects (vehicles) using background subtraction  
- To define parking slots using region-based annotation  
- To classify each parking slot as occupied or vacant  
- To visualize results in real time using bounding boxes  

---

## 3. Methodology

The system follows a structured pipeline based on classical computer vision techniques.

### 3.1 System Architecture & Tech Stack

- Programming Language: Python  
- Libraries: OpenCV, NumPy  
- Development Environment: VS Code  
- Input Source: CCTV video feed  
- Output: Real-time occupancy visualization  

---

### 3.2 Module Development (Input)

The system is divided into functional modules:

#### Video Preprocessing
- Convert frames to grayscale  
- Apply CLAHE for contrast enhancement  
- Apply Gaussian blur to reduce noise  

#### Background Subtraction
- Use MOG2 algorithm to separate foreground from background  
- Identify moving objects (vehicles)  

#### Slot Annotation
- Manual selection of parking slots using a click-based tool  
- Each slot represented as a polygon (ROI)  

---

### 3.3 Execution & Integration (Process)

The workflow integrates all modules into a pipeline:

1. Capture video frames  
2. Apply preprocessing  
3. Perform background subtraction  
4. Load predefined parking slots  
5. For each slot:
   - Create mask  
   - Calculate pixel density  
   - Classify occupancy  
6. Display results with colored bounding boxes  

---

### 3.4 Testing & Validation (Output)

The system will be evaluated using:

- Accuracy of slot classification  
- Stability of detection over time  
- Frame processing speed (FPS)  
- Behavior under different lighting conditions  

---

### 3.5 Constraints

- Performance may degrade under low lighting  
- Shadows may affect detection  
- Camera displacement requires recalibration  
- Static object detection is limited by background modeling  

---

## 4. System Pipeline

Video Input  
Preprocessing  
Background Subtraction  
Slot Detection  
Occupancy Classification  

---

## 5. Timeline

| Week | Task |
|------|------|
| 1-2 | Literature review and idea finalization |
| 3-4 | Video preprocessing implementation |
| 5-6 | Background subtraction |
| 7-8 | Slot detection and annotation |
| 9-10 | Occupancy classification |
| 11-12 | Testing and optimization |

---

## 6. Resources

- Python (OpenCV, NumPy)  
- CCTV video dataset  
- Personal computer for development  

No external funding required.

---

## 7. Future Work

- Improve detection for static vehicles  
- Multi-camera integration  
- Nearest parking slot recommendation  
- Mobile/web interface for user guidance  

---

## 8. Conclusion

This project demonstrates that parking slot detection can be achieved using classical computer vision techniques without relying on deep learning. The system is lightweight, cost-effective, and suitable for real-time applications using existing infrastructure.

---