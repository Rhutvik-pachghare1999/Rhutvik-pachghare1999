<!-- ================= HEADER ================= -->

<p align="center">
  <img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/Rhutvik-pachghare1999/main/image.jpg"
       alt="The Mechanica Library Robotics Banner" width="100%" />
</p>

<h1 align="center">🤖 Rhutvik Pachghare</h1>

<p align="center">
  <b>Robotics & Autonomous Systems Engineer</b><br/>
  Building health‑aware autonomy stacks for UAVs, satellites, and robotic fleets.
</p>

<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=Space+Mono&weight=600&size=22&pause=2000&color=3B82F6&center=true&vCenter=true&width=1000&lines=Robotics+%26+Autonomous+Systems+Engineer;UAV+Health+Monitoring+%26+Prognostics;Satellite+Mission+Control+%26+Telemetry;Safety-Critical+Robotics+Infrastructure"
    alt="Typing headline"
  />
</p>

---

<!-- ================= SKILLS ================= -->

<h2 align="center">⬣ Skills & Tools</h2>

<p align="center">
  <!-- Languages & OS -->
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
</p>

<p align="center">
  <!-- Robotics & Simulation -->
  <img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white" />
  <img src="https://img.shields.io/badge/NVIDIA%20Isaac%20Sim-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
  <img src="https://img.shields.io/badge/Robotics%20Simulation-0EA5E9?style=for-the-badge" />
</p>

<p align="center">
  <!-- ML & MLOps -->
  <img src="https://img.shields.io/badge/Time--Series%20ML-FF6F00?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Anomaly%20Detection-8A2BE2?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Deep%20Learning-20232A?style=for-the-badge&logo=pytorch&logoColor=EE4C2C" />
</p>

<p align="center">
  <!-- Systems & Dashboards -->
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/REST%20APIs-0052CC?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Telemetry%20Dashboards-0F766E?style=for-the-badge" />
</p>

<p align="center">
  <!-- Dev & Infra -->
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
</p>

---

## ⬣ Professional Overview

- Robotics & autonomous systems engineer focused on **UAVs, satellites, and mission‑critical robotic fleets**.  
- Designs end‑to‑end systems from **sensing and simulation** to **diagnostics, ML models, and operator dashboards**.  
- Especially interested in reliability, health monitoring, and safety for autonomous platforms.

---

## ⬣ Engineering Highlights

- 🛡️ Built **UAV health and prognostics** pipelines for propellers and motors using vibration signatures and deep learning models.  
- 🛰️ Prototyped **satellite mission‑control and health monitoring** stacks combining orbital dynamics, GNC hooks, and anomaly flags.  
- 📡 Designed **telemetry and MLOps workflows** that turn raw sensor data into actionable health indicators and dashboards.  
- 🧪 Developed **simulation‑driven workflows** with synthetic scenarios, domain randomization, and replayable logs for debugging.

---

## ⬣ Academic & Research Focus

- Safety‑critical autonomous systems and robotics health monitoring.  
- Time‑series analysis and ML for fault detection, anomaly detection, and Remaining Useful Life style metrics.  
- System design for observability: logging, metrics, and dashboards that help operators trust autonomy.

---

## ⬣ Core Technical Infrastructure

- **Languages & Core Tools**: Python, Git/GitHub, Jupyter, Linux.  
- **Robotics & Simulation**: ROS2, NVIDIA Isaac Sim, synthetic data generation, time‑series signal processing.  
- **ML for Robotics**: CNNs, RNN/LSTMs, anomaly detection (e.g., Isolation Forest), model evaluation and confusion‑matrix analysis.  
- **Systems & Dashboards**: Streamlit, REST/HTTP interfaces, config‑driven pipelines, structured logging, telemetry visualization.

---

## ⬣ Featured Projects

### 🤖 DriftBot — Autonomous Ground Robot with 360° ToF SLAM (ROS2)

From-scratch physical robot: ESP32-S3 dual-core firmware + ROS2 Jazzy micro-ROS pipeline.

- Custom rotating 3× VL53L1X ToF array assembled into 360° `LaserScan`; SLAM Toolbox mapping.
- Dual-core FreeRTOS firmware, dual I2C buses, EKF sensor fusion via robot_localization.
- Real recorded 90-min hardware session: **475,134 messages** across the full topic set (evidence in-repo).

🔗 Repo: [driftbot-ros2-slam](https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam)

---

### 🛡️ Autonomous Drone Safety Architecture — Real-Time Safety Kernel (C/C++)

Hard real-time safety kernel wrapping an AI-driven quadrotor stack: HOCBF safety filter, 15-state EKF, BFT consensus.

- Deterministic C safety filter that clamps actuator commands; CI-tested.
- Honest status accounting (implemented / tested / planned); formal FSM/Z3 verification is specified and planned, not yet proven.

🔗 Repo: [autonomous-drone-safety-architecture](https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture)

---

### 🔎 Edge Detection Active Learning — Label-Efficient Object Detection Benchmark

Rigorous, leakage-free active-learning benchmark on COCO-2017 (RT-DETR teacher → YOLOv8n student).

- Evaluated against **held-out human labels**, never the teacher's guesses; train/test disjointness is test-enforced.
- Reports a clean positive result (entropy sampling beats random) **and** an honest negative result (teacher-student disagreement does not).
- CI-enforced test suite.

🔗 Repo: [edge-detection-active-learning](https://github.com/Rhutvik-pachghare1999/edge-detection-active-learning)

---

### 🛡️ UAV Aegis — UAV Propeller Fault Diagnostics (ROS2 + Deep Learning)

Propeller/motor fault diagnostics from high-frequency vibration signatures: 1D-CNN classifier, FFT features, LSTM RUL.

- Supports propulsion health assessment and maintenance analysis; ROS2 inference node + Streamlit dashboard.
- Headline accuracy is reported from training runs; sealed episode-level held-out evaluation is in progress (documented honestly in-repo).

🔗 Repo: [uav-fault-diagnostics-ros2](https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2)

---

### 🧠 NeuroTraction — Real-Time ML Traction Control for Ground Robots (ROS2)

Real-time slip prediction that throttles velocity commands before traction is lost.

- Lightweight MLP predicts wheel slip from IMU + odometry inside a 20Hz ROS2 safety node.
- **0.945 held-out R²** on a leakage-free split (scaler fit on training data only); a `pytest` leakage guard runs in CI.

🔗 Repo: [neurotraction-ros2-slip-control](https://github.com/Rhutvik-pachghare1999/neurotraction-ros2-slip-control)

---

## ⬣ What I’m Looking For

- **Robotics Engineer / Robotics Infrastructure Engineer** roles on UAV, satellite, or robotic fleet teams.  
- **Autonomous Systems / Perception & Diagnostics Engineer** positions focused on reliability, health monitoring, and safety.  
- Teams that value **simulation, observability, and mission‑critical robustness** as much as raw model performance.
