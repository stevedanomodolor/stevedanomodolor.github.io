---
layout: page
title: Pose Estimation and Position-based Visual-servoing
description: The project consist  developing a strategy to control the position of the end-effector and the mobile base od the Tiago robot using visual servoing feedback from a stereo camera. 
img: assets/img/visual_servoing.png
importance: 1
category: general
related_publications: true
---

The idea of visual servoing consist of controlling the motion of a robot using information obtained from a computer vision feedback system. The visual data can come from a camera placed directly on the the robot’s end-effector(eye-in-hand configuration) or placed in a fixed position in the work space(fixed-camera configuration). The basic ideal of visual servoing consists of the minimization of an error value. The different visual-servoing techniques. differ with respect to the error function defined. In position-based image visual seroving(PBVS), the error function is specified based on position value in the robot task space. In Image-Based Visual servoing, the error function is defined in terms of image features. Although, IBVS is considered favorable compared to PBVS due to it low sensitivity to camera calibration errors, PBVS method was used. This is due to the limitation with respect to the control layer of the Tiago robot {% cite VisualServoing %}.

 
The following shows one of the video experiments obtained during the project: 

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/visual_servoing.mp4" title="Servo-image" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Demostration using the visual servoing technique
</div>





Some of the results of the experiments performed can be found below:


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/code_design.png" title="Schematic of the code design." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Schematic of the code design
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-2 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/feature.png" title="Image after obtaining the feature point and contours" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Image after obtaining the feature point and contours
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/visual_servoing.png" title=" Initial configuration of the robot" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Initial configuration of the robot
</div>

