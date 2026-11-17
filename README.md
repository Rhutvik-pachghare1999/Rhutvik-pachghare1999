# Rhutvik Pachghare

**Robotics engineer | ROS 2, controls, perception, and robot learning**

Hi, I'm Rhutvik. I work on the part of robotics where software has to answer to physics. I've worked on quadrotor control, fault detection, SLAM, and mobile robot perception. What interests me most is finding out whether something *actually works*, not just whether it looks good in a demo.

I earned my M.S. in Robotics and Autonomous Systems at Arizona State University. These days I'm also building toward a robotics startup focused on testing, diagnosing, and improving learned robot behavior.

## A few projects

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture/main/experiments/results/crazyflie_vla_iso500.png" alt="Isaac Sim paired test of a quadrotor safety filter" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture">Keeping unsafe commands away from a quadrotor</a></h3>
<p>A controller should have a say when a high-level model asks a drone to do something unsafe. I built an HOCBF thrust filter and tested it with deliberately unsafe descent commands.</p>
<p>In <strong>500 paired Isaac Sim episodes</strong>, the filtered controller avoided ground impact in all 500; the unfiltered controller did not.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture/blob/main/experiments/results/crazyflie_vla_iso500.json">Results</a> · <a href="https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture#build-test-reproduce">Build and test</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/main/results/figures/fig6_cross_speed.png" alt="Rotor-fault classification across held-out RPM bands" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2">Finding rotor faults from IMU data</a></h3>
<p>I injected rotor faults into simulated Crazyflie flights, trained a CNN on 0.2-second IMU/RPM windows, and built a ROS 2 inference path.</p>
<p>The classifier reached <strong>81.7% accuracy on 32 held-out simulated flights</strong>. The repo includes the split protocol, evaluation artifacts, and code.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/tree/main/results/eval_sealed">Evaluation</a> · <a href="https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2/blob/main/reproduce.sh">Reproduction pipeline</a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/driftbot-ros2-slam/main/docs/img/slam_map_sim.png" alt="Jackal SLAM map and trajectory against Gazebo ground truth" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam">Checking SLAM against ground truth</a></h3>
<p>DriftBot runs a Jackal with ROS 2 Jazzy, Gazebo, an EKF, and SLAM Toolbox. Instead of judging the map by eye, I compare it with the simulator's geometry and ground-truth trajectory.</p>
<p>The published scripted run recorded <strong>5.7 cm EKF trajectory RMSE</strong>. I also kept a separate headless replay.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam/blob/main/docs/maps/replication_20261117.json">Replay results</a> · <a href="https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam#quick-start">Run it</a></p>
</td>
<td width="50%" valign="top">
<a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot"><img src="https://raw.githubusercontent.com/Rhutvik-pachghare1999/assistive-follower-robot/master/docs/results/lidar_gap_real.png" alt="Real LiDAR scan and Follow Gap processing" width="100%"></a>
<h3><a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot">A TurtleBot that follows a person</a></h3>
<p>For an ASU team project, we combined OAK-D shoe detection with LiDAR-based obstacle avoidance on a TurtleBot 4. I worked on the detection model, ROS 2 integration, and deployment.</p>
<p>The repository includes real sensor captures, model results, launch files, and the ROS 2 nodes.</p>
<p><a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot/tree/master/docs/results">Sensor captures</a> · <a href="https://github.com/Rhutvik-pachghare1999/assistive-follower-robot/tree/master/my_nodes">Code</a></p>
</td>
</tr>
</table>

I also built [EdgeAL](https://github.com/Rhutvik-pachghare1999/edge-detection-active-learning), where I compared annotation strategies on COCO rather than assuming a more complicated method would win; [NeuroTraction](https://github.com/Rhutvik-pachghare1999/neurotraction-ros2-slip-control), a ROS 2 wheel-slip control prototype; and a [robotics evaluation framework](https://github.com/Rhutvik-pachghare1999/robotics-eval-framework) for keeping test evidence traceable.

## What I'm working on now

I'm interested in a question that keeps coming up as robots learn more of their behavior: **how do you know a new skill or policy is better before you put it on a robot?**

My current startup work is around that problem: repeatable evaluation, failure diagnosis, and making robot skills easier to improve and maintain. If you're building or deploying robot systems, I'd like to compare notes.

[Portfolio](https://port-web-891m.onrender.com/) · [LinkedIn](https://www.linkedin.com/in/rhutvik-pachghare/) · [Email](mailto:rhutvik012@gmail.com)
