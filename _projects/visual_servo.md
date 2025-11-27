---
layout: page
title: Visual Servo
description: .
img: assets/img/visual_servo/visualservo_go2.png
importance: 4
category: fun
related_publications: false
---

For my university image processing class, I created a fun project called "Visual Servo." The goal was to develop a system that uses computer vision to control and guide a robot or device based on visual feedback. I implemented basic image processing techniques to detect and track the poisition of the red ball in real time. The control of Z1 manipulator arm is handled by [Moveit2](https://moveit.picknik.ai/main/index.html). The below video is conducted in Gazebo simulation.

<!-- <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/lunar_rough.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/lunar_rough2.mp4" class="img-fluid rounded z-depth-1" autoplay=true loop=true %}
    </div>
</div> -->

The core method involved using color segmentation and contour detection to identify the target object in the camera feed. Once detected, the system calculated the object's position and sent commands to adjust the manipulator arm movement, keeping the target centered in view. This hands-on project helped me understand practical applications of image processing and control systems, especially the usage of OpenCV and Moveit2. and it was a rewarding experience to see theory come to life through experimentation.