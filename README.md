# Rhutvik Pachghare

Robotics & Autonomous Systems Engineer. I build the layers between a learned
model and the hardware it can hurt: state estimation, fault diagnostics, and a
safety filter that gets the last word on any command.

MS in Robotics and Autonomous Systems, Arizona State University. Graduate
researcher on the ASU + Barrow Neurological Institute lumbar-spine MRI project.

Most of what's here is one specialization seen from four angles: perception,
estimation, fault awareness, and safety enforcement.

## Projects

**Safety enforcement — [autonomous-drone-safety-architecture](https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture)**
Every command from an RL policy or a vision-language model passes through a closed-form HOCBF filter before the motors. C/C99 hot path, no solver in the loop.

- 500 paired Isaac Sim episodes on the Crazyflie 2.X: filter on survived 500/500, filter off crashed 500/500. Identical controller; only the projection differs.
- Observed max filter latency 2,725 ns over 100,000 cycles against a 100 µs budget (p99: 31 ns).
- EKF gating, HMAC-authenticated swarm consensus, and a live rendered-camera VLA loop (216/216 structured parses, zero crashes).
- Simulation only, not certified, formal verification planned — stated in the repo.
- [Project poster](https://rhutvik-pachghare1999.github.io/autonomous-drone-safety-architecture/)

**Fault awareness — [uav-fault-diagnostics-ros2](https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2)** (UAV Aegis)
Classifies which rotors are faulted on a Crazyflie 2.1 from 0.2 s IMU + RPM windows. 112K-parameter CNN on 96 fault-injected Isaac Sim flights at 500 Hz.

- 81.7% on a sealed test set of 32 untouched flights (35,232 windows); healthy-flight F1 is 1.00 — no false alarms, no missed faults on that set.
- 93.2% mean accuracy holding out an entire hover-RPM bin per fold (4 folds, retrained each time).
- Out-of-distribution windows flagged at AUROC 0.996; 0.37 ms p99 inference on CPU; deploys as a single ROS 2 Jazzy node that refuses to run on invalid inputs.
- The honest corner: the R3+R4 fault pair reaches 0.13 recall at low RPM, and everything is simulation-only.

**State estimation — [driftbot-ros2-slam](https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam)**
Reproducible SLAM evaluation on a simulated Clearpath Jackal: Gazebo Harmonic, robot_localization EKF, slam_toolbox, Nav2.

- 5.7 cm trajectory RMSE over an 8.96 m scripted drive (1,565 synced samples).
- Map vs continuous ground-truth surfaces: 2.7 cm precision, 99.8% surface recall, zero spurious obstacles.
- Published benchmark is teleop-only; the Nav2 autonomous demo is blocked by a documented TF time-sync issue in Gazebo. Both facts are in the README.

**Slip estimation — [neurotraction-ros2-slip-control](https://github.com/Rhutvik-pachghare1999/neurotraction-ros2-slip-control)**
A small MLP reads IMU + wheel odometry inside a ROS 2 safety node and scales velocity commands before traction is lost (IMU-rate, ≤20 Hz).

- ~99.4% binary grip/slip accuracy on a per-recording strided hold-out, scaler fit on train rows only.
- Three scripted runs total — a working prototype, not a generalization claim. See "Numbers I got wrong" below.

**Evaluation honesty — [edge-detection-active-learning](https://github.com/Rhutvik-pachghare1999/edge-detection-active-learning)** (EdgeAL)
Active-learning benchmark for edge object detection on COCO-2017 (RT-DETR teacher, YOLOv8n student), scored against held-out human labels.

- At 2% and 4% label budgets, random sampling was the strongest baseline; the uncertainty strategies tested did not beat it.
- 76 tests plus one data-gated skip run in CI on every push.

**Medical imaging — [bni-asu-lumbar-stenosis-asd](https://github.com/Rhutvik-pachghare1999/bni-asu-lumbar-stenosis-asd)**
ASU + Barrow Neurological Institute statement-of-work pipeline: multi-task ConvNeXt-Tiny diagnosing five lumbar-stenosis conditions on RSNA 2024 MRI, with external validation on a Barrow cohort.

- Phase 1 code is complete and audit-remediated; final metrics wait on the full A100 cluster run, so there is no accuracy number to cite yet.
- Every result carries git SHA + config, manifest, and checkpoint hashes.
- Poster presented at the ASU Forge Research Expo 2026.

**Team hardware — [assistive-follower-robot](https://github.com/Rhutvik-pachghare1999/assistive-follower-robot)**
RAS 598 Team 07 (with Mohammad Nasr and Shashank Sing Deo): a TurtleBot 4 that follows a person by detecting their shoes (OAK-D + ResNet18) and steering through the widest LiDAR gap.

- My part: detection model, ROS 2 integration, deployment. 15 ms per frame on a Raspberry Pi 4; 95% follow success around static obstacles, 87% with people moving through.
- SLAM + Nav2 never ran stably on the physical robot, so we shipped reactive gap-following instead. That tradeoff is written up in the repo.

## Numbers I got wrong

- NeuroTraction first reported R² 0.9912 with a scaler fit on the full dataset. That was leakage. The corrected number, R² 0.9999, is leakage-free but comes from held-out rows 0.05 s from training rows — interpolation on three easy runs, not generalization. Both numbers stay in the repo as a record of the mistake.
- UAV Aegis once reported 99.0% test accuracy from a non-frozen split. Rebuilding the pipeline around a sealed, sha256-pinned flight-level split put it at 81.7%. The 81.7 is the number I cite.

## Contact

Open to full-time robotics and autonomy roles. I respond within a day.

Portfolio: https://port-web-891m.onrender.com/ · LinkedIn: https://www.linkedin.com/in/rhutvik-pachghare/ · Email: rhutvik012@gmail.com
