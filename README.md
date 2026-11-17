# Rhutvik Pachghare

**Robotics engineer · ROS 2, robot learning, controls & autonomy**

I build robot systems and the tools to measure whether they work: control and safety layers, state estimation, perception, failure diagnosis, and reproducible simulation. I have an M.S. in Robotics and Autonomous Systems from Arizona State University.

I'm also working toward a robotics company focused on making learned robot behavior easier to test, diagnose, and improve.

## Engineering work

These are working implementations with source code, experiment artifacts, and ways to reproduce the results—not just project concepts.

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture/main/experiments/results/crazyflie_vla_iso500.png" alt="Paired Crazyflie simulation evaluation of a control barrier function safety filter" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture">Drone safety architecture</a></h3>
<p>C++/Python higher-order control barrier function filter for unsafe drone commands, with estimator and watchdog integration.</p>
<p><strong>500/500 protected episodes</strong> in a paired Isaac Sim adversarial-descent experiment.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture/blob/main/experiments/results/crazyflie_vla_iso500.json">Experiment data</a> · <a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture/tree/main/tests">Tests</a> · <a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture#build-test-reproduce">Reproduce</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/main/results/figures/fig6_cross_speed.png" alt="Held-out flight RPM band fault classification benchmark" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2">UAV Aegis — fault diagnostics</a></h3>
<p>Fault-injected flight data, an IMU/RPM CNN classifier, sealed evaluation, and a ROS 2 inference node.</p>
<p><strong>81.7% classification accuracy</strong> on 35,232 windows from 32 held-out simulated flights; separately evaluated speed-bin generalization.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/tree/main/results/eval_sealed">Evaluation</a> · <a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/blob/main/reproduce.sh">Pipeline</a> · <a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/tree/main/tests">Tests</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/driftbot-ros2-slam/main/docs/img/slam_map_sim.png" alt="Jackal SLAM map with EKF trajectory and Gazebo ground-truth reference" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam">DriftBot — SLAM & localization</a></h3>
<p>Jackal, Gazebo Harmonic, ROS 2 Jazzy, EKF, SLAM Toolbox, and ground-truth map evaluation.</p>
<p><strong>5.7 cm EKF trajectory RMSE</strong> in the published simulated scripted-drive benchmark; independently replayed headlessly.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam/blob/main/docs/maps/replication_20261117.json">Independent replay</a> · <a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam/blob/main/scripts/sim_e2e_run.py">Evaluator</a> · <a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam#quick-start">Run</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/assistive-follower-robot/master/docs/results/lidar_gap_real.png" alt="Measured LiDAR scan and obstacle-free gap selection from TurtleBot follower project" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot">Assistive follower robot</a></h3>
<p>Team-built TurtleBot 4 system combining OAK-D visual shoe detection, LiDAR Follow Gap navigation, and ROS 2 integration.</p>
<p><strong>Hardware and perception integration</strong>, including detector inference, real LiDAR traces, and robot-side deployment.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot/tree/master/docs/results">Hardware evidence</a> · <a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot/tree/master/my_nodes">ROS 2 code</a> · <a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot#quick-start">Build</a></p>
</td>
</tr>
</table>

### More engineering

- **[EdgeAL](https://github.com/Rhutvik-pachghare1999/edge-detection-active-learning)** — controlled COCO object-detection active-learning experiments and evaluation tooling, with [benchmark visualizations](https://github.com/Rhutvik-pachghare1999/edge-detection-active-learning/tree/master/docs/figures).
- **[Robot evaluation framework](https://github.com/Rhutvik-pachghare1999/robotics-eval-framework)** — machine-checkable experiment manifests, result provenance, and validation guards.
- **[NeuroTraction](https://github.com/Rhutvik-pachghare1999/neurotraction-ros2-slip-control)** — ROS 2 wheel-slip prediction and velocity adaptation.

## What I'm building toward

Reliable learned autonomy requires more than training a policy. I'm interested in the engineering layer between a model checkpoint and a robot that can be trusted in a customer workflow: repeatable evaluation, useful diagnostics, and evidence-based improvement.

I enjoy discussing real robotics problems with engineers, researchers, and teams deploying autonomous systems.

[**Portfolio & case studies**](https://port-web-891m.onrender.com/) · [**LinkedIn**](https://www.linkedin.com/in/rhutvik-pachghare/) · [**Email**](mailto:rhutvik012@gmail.com)
