---
layout: page
title: Head and gaze tracking control
description: Head and gaze tracking control for a smart wheelchair with a robot arm
img: assets/img/head_and_gaze.png
importance: 2
category: work
related_publications: true
---

For people with severe disabilities who do not suit with conventional
wheelchair driving systems, like the manual ones or the electric with
joysticks, for example; alternatives and solutions have been researched,
leading to a proposal that has been developed based on an interface that
simulates the control of a wheel-driven platform, such as a wheelchair,
with an integrated robotic arm, both controlled by head gestures and gaze
tracking. A webcam and a facial recognition algorithm are used to read
the input movements, and a simulation program to perform the actions{% cite finaldemo %}

The following shows the system design schematics ad the simulation environment: 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/system_design_head_tracking.png" title="Free-space UAV Formation and Flocking" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    System design and simulation environment
</div>

The final video demostration of this project can be seen below:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/head_and_tracking.mp4" title="example image" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Video demostration
</div>



Full implementation of the code can bge found [here](https://github.com/stevedanomodolor/Head_and_gaze_tracking_control_for_a_smart_wheelchair_with_a_robot_arm/tree/master)
