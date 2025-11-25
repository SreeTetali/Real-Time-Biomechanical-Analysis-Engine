# Real-Time-Biomechanical-Analysis-Engine
Real-Time Biomechanical Analysis Engine

# Deadlift Decoded: Real-Time Biomechanical Analysis Engine 🏋️‍♂️👁️

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Computer Vision](https://img.shields.io/badge/Computer_Vision-MediaPipe_OpenCV-green)]()
[![Status](https://img.shields.io/badge/Status-Research_Complete-orange)]()

### 🚀 Executive Summary
**Deadlift Decoded** is an AI-powered coaching system that utilizes Computer Vision (CV) to perform real-time ergonomic analysis. By leveraging **MediaPipe** for high-fidelity pose estimation and geometric vector analysis, this system democratizes professional-grade biomechanics coaching. It operates with low latency on standard hardware, making it a scalable solution for HealthTech and Fitness applications.

> **Why this matters:** Improper weightlifting form is a leading cause of lumbar injuries. This project solves the "feedback loop" problem by providing instant, automated correction without the need for human intervention.

### 🎥 Demo / Visualization
*(Ideally, put a GIF here of the code detecting a skeleton on a video)*
![System Architecture](https://via.placeholder.com/800x400?text=Insert+Screenshot+of+Skeleton+Overlay+Here)

### 🧠 Key Technical Innovations
* **Human Pose Estimation:** Implemented **MediaPipe** to extract 33-point skeletal landmarks with sub-millisecond inference time.
* **Vector Geometry Analysis:** Developed custom algorithms to calculate dynamic joint angles (Hip-Shoulder-Knee relationships) in 2D space.
* **State Machine Logic:** Engineered a robust finite-state machine to automatically detect lift phases (Setup $\to$ Pull $\to$ Lockout) without user input.
* **Real-Time Feedback Loop:** Built a visual overlay engine using **OpenCV** to provide "Pass/Fail" cues instantly to the user.

### 🛠️ Tech Stack
* **Language:** Python
* **Vision Library:** OpenCV, Google MediaPipe
* **Math/Logic:** NumPy, Trigonometry (Vector Calculus)
* **Visualization:** Matplotlib (for post-lift analytics)

### ⚙️ How It Works (The Algorithm)
1.  **Input:** Ingests video stream (Webcam or File).
2.  **Inference:** MediaPipe model infers skeletal coordinates $(x, y, z)$.
3.  **Calculation:**
    * *Back Angle:* Computed relative to the vertical axis.
    * *Neck Alignment:* Computed relative to the torso vector.
4.  **Decision Engine:** If angles deviate from safe biomechanical thresholds (>15 degrees curvature), the system triggers an alert.
5.  **Output:** Rendered overlay on the video frame.

### 🌐 Scalability & Industry Applications
While developed for weightlifting, this **Ergonomic Monitoring Framework** is transferable to high-value sectors:
* **Physical Therapy:** Automated range-of-motion tracking for patient recovery.
* **Industrial Safety:** Monitoring factory workers for unsafe lifting posture to reduce workman's comp claims.
* **Elderly Care:** Fall detection and gait analysis.

### 📄 Research Paper
* [**Read the Full Research Paper (PDF)**](./Deadlift_Decoded.pdf) - Includes detailed methodology, mathematical thresholds, and accuracy results.

---
*This research was conducted as a collaborative capstone project in Computer Vision.*
