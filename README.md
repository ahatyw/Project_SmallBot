# Project SmallBot 🤖  
### A Research-Oriented Multi-Modal Human–Robot Interaction Platform

**Author:** Aniket Agarwal  
**Degree:** B.Tech Computer Science Engineering  
**Institution:** Amity University Punjab, India  

---

## 📌 Overview

**Project SmallBot** is a **software-first, research-oriented robotic platform** designed to explore how humans can interact naturally with autonomous machines using **gesture**, **voice**, and **autonomous behaviors** within a unified control architecture.

Rather than focusing on hardware novelty, this project emphasizes:

- Human–Robot Interaction (HRI)
- Interaction logic and intent abstraction
- Modularity and extensibility
- System transparency and explainability

The system acts as a **research testbed** for future work in **intelligent autonomy, adaptive interaction, and explainable robotics** :contentReference[oaicite:0]{index=0}

---

## 🎯 Core Research Idea

> **What if a robot could understand human intent using the same channels humans naturally use — movement, speech, and proximity — while remaining transparent about its internal state?**

Project SmallBot treats **gesture control**, **voice commands**, and **autonomous navigation** as **parallel expressions of human intent**, all feeding into a **single unified decision pipeline** instead of isolated control systems :contentReference[oaicite:1]{index=1}

---

## 🧠 Key Research Questions

- Can spatial gesture interaction improve intuitive robot navigation?
- How can voice commands and API-based control coexist cleanly?
- How does expressive feedback influence user trust and system transparency?
- Can interaction logic be decoupled from embedded hardware for scalability?

---

## 🏗️ System Architecture

This separation allows **independent evolution of interaction modules** without breaking the system :contentReference[oaicite:2]{index=2}

---

## 🔧 Feature Design & Rationale

### ✋ Gesture-Based Spatial Control
- Uses **vision-based hand tracking**
- Divides camera frame into spatial zones
- Direction is inferred from hand position, not symbolic gestures

**Why this approach?**
- Lower computational complexity
- Reduced false positives
- More intuitive human guidance
- Robust under real-world lighting conditions

---

### 🎤 Voice Commands as Intent Abstractions
- Voice commands represent **high-level intent**
- Commands are mapped to standardized software actions
- No direct motor-level voice control

This abstraction ensures **safety, consistency, and extensibility**.

---

### 🚗 Autonomous Obstacle Avoidance
- Reactive autonomy using ultrasonic sensors
- Manual inputs are ignored when autonomy is active
- Predictable and conflict-free behavior

---

### 👀 Expressive OLED Feedback
- OLED display shows symbolic “eyes” and states
- Communicates robot intent and status visually
- Improves user trust and system transparency

---

## 🧩 Unified Command Pipeline

All interaction modalities follow the same logical flow:

1. Capture human input  
2. Interpret intent  
3. Normalize into a command  
4. Transmit via REST API  
5. Execute on embedded system  
6. Reflect state visually  

This prevents fragmented logic and conflicting behaviors :contentReference[oaicite:3]{index=3}

---

## 🔄 State-Based Execution Model

The robot operates using explicit internal states:

- **Manual Control**
- **Autonomous Navigation**
- **Idle / Emergency Stop**

State transitions are strictly enforced to avoid ambiguity.

---

## 💻 Technologies Used

| Domain | Technologies |
|------|-------------|
| Embedded Control | Arduino C++, ESP32 Wi-Fi Stack |
| Vision Processing | Python, OpenCV, CVZone |
| Voice Interface | SpeechRecognition |
| GUI / Control | PyQt |
| Networking | REST APIs, HTTP |
| Visualization | OLED Graphics Libraries |

---

## 🧪 Research Contributions

This project contributes:

- A **modular, network-driven robotic control architecture**
- A **multi-modal HRI framework** (gesture + voice + autonomy)
- An **expressive feedback mechanism** for transparency
- A **reusable experimental platform** for HRI research :contentReference[oaicite:4]{index=4}

---

## 🚀 Future Research Directions

### 🤖 Learning-Based Gesture Interpretation
- Replace spatial heuristics with neural networks
- Enable dynamic and personalized gestures

### 🧠 Adaptive Human–Robot Interaction
- Reinforcement learning for behavior adaptation
- Improved trust and efficiency

### 🗺️ Vision-Based Navigation & SLAM
- Environment mapping
- Goal-directed autonomy

### ☁️ Cloud-Integrated Robotics
- Shared learning between multiple robots
- Remote supervision and analytics

### 🔍 Explainable Robot Decision-Making
- Visualizing reasoning processes
- Improving transparency and acceptance

---

## 📊 Proposed Evaluation Methodology

Future experiments may evaluate:

- Task completion time across modalities
- User intuitiveness and cognitive load
- Obstacle avoidance success rate
- Robustness of autonomous behavior

---

## 🌱 Why This Project Matters

Project SmallBot demonstrates that **impactful robotics research can emerge from thoughtful system design**, not just hardware complexity.

It serves as:

- A **Human–Robot Interaction research testbed**
- A **learning platform for modular robotics**
- A **software-first robotics architecture**
- A **foundation for explainable and adaptive autonomy** :contentReference[oaicite:5]{index=5}

---

## 📌 Closing Note

> **Project SmallBot is not an endpoint — it is a research instrument.**

The system is intentionally open-ended, designed to evolve with future learning-based, adaptive, and explainable robotic intelligence.

---




The system follows a **layered, modular architecture**:

