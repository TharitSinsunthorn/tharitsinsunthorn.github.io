---
layout: page
title: Moonbot 0
description: Self-recognition for Modular Legged Robot.
img: assets/img/bachelor_thesis/moonbot0.png
importance: 2
category: work
related_publications: true
---
Moonbot is a prototype of modular legged robot of [Moonshot project Goal 3B](https://srl-moonshot.mech.tohoku.ac.jp/research_1.html), designed for the challenges of lunar exploration. Unlike traditional robots with fixed structures, Moonbot can dynamically change its configuration by attaching or detaching leg modules.

The core of this project is a **self-recognition algorithm** {% cite Danish Ai2024 %} that allows the robot to understand its own structure in real-time. Based on the number of legs connected, Moonbot automatically adapts its motion control strategy. This enables a single robotic platform to perform various tasks with different levels of mobility and stability.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bachelor_thesis/selfrecog.gif" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/bachelor_thesis/selfrecog2.gif" %}
    </div>
</div>
<div class="caption">
    Moonbot adapting its locomotion style based on its configuration.
</div>

For example:
*   With one or two legs, Moonbot uses a **crawling motion** to move, similar to an inchworm.
*   In a full four-legged configuration, it switches to a more stable and efficient **walking gait**.

The entire system is built on ROS 2, ensuring a robust and scalable software foundation. This project demonstrates the potential of modular, self-aware robots for future space exploration missions.

