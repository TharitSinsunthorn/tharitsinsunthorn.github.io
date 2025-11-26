---
layout: page
title: Moonbot 0
description: Self-Recognition for a Modular Legged Robot.
img: assets/img/bachelor_thesis/moonbot0.png
importance: 2
category: work
related_publications: true
---
Moonbot is a prototype of a modular legged robot from [Moonshot project Goal 3B](https://srl-moonshot.mech.tohoku.ac.jp/research_1.html), designed for the challenges of lunar exploration. The key concept of Moonbot is the dynamic adaptation of its configuration by attaching or detaching modules.

The entire system is built on ROS2, combined with the [Dynamixel SDK](https://emanual.robotis.com/docs/en/software/dynamixel/dynamixel_sdk/overview/) hardware interface. The core part of the project is a **self-recognition algorithm** {% cite DanishAi2024 %} that allows the robot to detect its own structure in real-time. Based on the number of connected legs, Moonbot automatically adapts its motion control strategy.  In other words, this prototype showcases a single robotic platform that can perform various tasks with different levels of mobility and stability.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/inc.mp4" 
        class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/dec.mp4" 
        class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    Moonbot adapting its locomotion style based on its configuration.
</div>

For example:
*   With one or two legs, Moonbot uses a **crawling motion**, similar to an inchworm.
*   In a four-legged configuration, it switches to a more stable and efficient **walking gait**.

In addition, different kinds of modules, like a **gripper module**, can be attached. This transforms the robot from a purely mobile platform into a functional manipulator.

<div class="row justify-content-sm-center mt-3">
    <div class="col-sm-6">
        {% include video.liquid path="assets/video/grp.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    Demonstration of swapping from leg module to gripper module.
</div>