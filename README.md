# Rhutvik Pachghare

I'm a robotics engineer working on the boundary between learned autonomy and the physical systems it controls: state estimation, control, fault diagnosis, and repeatable evaluation.

M.S. in Robotics and Autonomous Systems, Arizona State University. I work primarily with ROS 2, Python/C++, Gazebo, Isaac Sim, and robot learning tools.

I'm also exploring a startup around a practical robotics problem: making new robot skills less costly to test, deploy, and maintain. That work is still at the research and customer-discovery stage. The public projects below show the engineering I've actually done.

## Selected engineering work

- **[Autonomous drone safety architecture](https://github.com/Rhutvik-pachghare1999/autonomous-drone-safety-architecture)** — A control-barrier-function filter between learned commands and a simulated Crazyflie. In one defined 500-pair Isaac Sim stress test, the filtered controller avoided the crash condition in all 500 trials; the unfiltered controller did not. **Simulation only, not a hardware safety certification.**
- **[UAV Aegis: fault diagnostics](https://github.com/Rhutvik-pachghare1999/uav-fault-diagnostics-ros2)** — Physics-based rotor fault injection, IMU/RPM classification, and ROS 2 deployment code. **81.7%** on the documented sealed, flight-separated simulation test set, with important weak classes reported.
- **[DriftBot: ROS 2 SLAM evaluation](https://github.com/Rhutvik-pachghare1999/driftbot-ros2-slam)** — Jackal, EKF, SLAM Toolbox, and Gazebo. **5.7 cm** trajectory RMSE on a scripted simulation run. Autonomous Nav2 performance is not included in that benchmark.
- **[EdgeAL: active-learning benchmark](https://github.com/Rhutvik-pachghare1999/edge-detection-active-learning)** — Compared image-selection methods on COCO using held-out human labels. At the evaluated 2% and 4% budgets, **random sampling was a stronger baseline** than the tested uncertainty methods. I kept the negative result.
- **[Assistive follower robot](https://github.com/Rhutvik-pachghare1999/assistive-follower-robot)** — Team-built TurtleBot 4 that follows a person using OAK-D vision and LiDAR obstacle avoidance. My work covered the detection model, ROS 2 integration, and deployment.

More work: [evaluation provenance framework](https://github.com/Rhutvik-pachghare1999/robotics-eval-framework) · [wheel-slip control](https://github.com/Rhutvik-pachghare1999/neurotraction-ros2-slip-control) · [research on lumbar MRI](https://github.com/Rhutvik-pachghare1999/bni-asu-lumbar-stenosis-asd).

## How I approach robotics

I care about whether a system works outside its easiest demonstration. I try to keep simulation results separate from hardware results, check against independent ground truth where possible, and document the cases that fail.

If you're working on robot reliability, manipulation, or learned autonomy, I'd be interested in comparing approaches.

[Portfolio](https://port-web-891m.onrender.com/) · [LinkedIn](https://www.linkedin.com/in/rhutvik-pachghare/) · [Email](mailto:rhutvik012@gmail.com)
