---
layout: page
title: RL Locomotion
description: Locomotion policy for quadruped robot in low-gravity env.
img: assets/img/master_thesis/go2_rl.png
importance: 1
category: work
related_publications: false
---

Here is my research and development of a reinforcement learning-based locomotion policy for quadruped robots. The main focus of this work is to enable adaptable and efficient movement on rough terrain in low-gravity environments, such as the lunar surface environment.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/lunar_rough.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/lunar_rough2.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    Simulations of the learned locomotion policy on a Unitree Go2 robot in a low-gravity, rough-terrain environment. The robot's gait (blue arrow) follows the commanded velocity (green arrow).
</div>

This project utilizes NVIDIA's [Isaac Lab](https://github.com/isaac-sim/IsaacLab) to train a locomotion policy for a quadruped robot using the Proximal Policy Optimization (PPO) algorithm. As shown in the simulations, the robot learns to generate a stable gait (indicated by the blue arrow) that follows the desired command velocity (green arrow), enabling it to navigate challenging, low-gravity terrain.
