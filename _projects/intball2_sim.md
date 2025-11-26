---
layout: page
title: Int-Ball2 Digital Twin
description: A digital twin of the JEM Internal Ball 2 in Isaac Sim.
img: assets/img/intball2_sim/intball2_sim.png
importance: 3
category: work
related_publications: true
---

As I had a chance to join the [Innovation team of Spacedata Inc.](https://spacedata.jp/news/2519_innovation_team_1). I was responsible for space robotics simulation development. So this project involved the creation of a photorealistics simulation environment for the **JEM Internal Ball Camera 2 (Int-Ball2)**, a free-flying camera robot used inside the Japanese Experiment Module "Kibo" on the International Space Station (ISS). The goal was to develop a digital twin of the robot using NVIDIA Isaac Sim.

<div class="row justify-content-sm-center mt-3">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/intball2_sim/intball2_sim2.png" title="Int-Ball2 Isaac sim" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Int-Ball2 Isaac sim simulation.
</div>

Key responsibilities included:
*   **Simulation Environment:** Architecting and implementing the core simulation environment in Isaac Sim, which represents the physical dynamics of the Int-Ball2 operating within the ISS-Kibo module.
*   **ROSbag Replay Functionality:** Another key feature that I implemented is developing a ROS2 package to process and republish rosbag files recorded from the actual Int-Ball2 on the ISS to feed real-world sensor data and commands into the simulation and analyze the differences between the simulated and physical robot's behavior, which is a core concept of a digital twin.

The github of the project is available here {% cite spacedata_intball2_github %}