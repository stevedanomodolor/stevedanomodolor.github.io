---
layout: page
title: Force and Torque Control of the Pr2 Robot
description: The project consist of upgrading the motor drivers on the pr2 to allow force/torque control through Ethercat protocol
img: assets/img/pr2.jpg
importance: 1
category: general
related_publications: true
---

While working as a reasearch assitant at the Robotic research group KU Leuven, I worked on updgrading the PR2 robots arm to use EtherCat Compliant drivers under Prof. Dr. Ir. Herman Bruyninckx. The integration was done using SOEM library(https://github.com/OpenEtherCATsociety/SOEM) to allows communication from the drivers to the pr2 robot motors. The end goal was to allow force and torque control of the robot arm using petrinet based state machines to allow real-time control. More info can found in the appendix of the reference{% cite Omodolor_2020%}.

 
The following video shows one of the video experiments obtained during the project: 
<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/pr2_moving.mp4" title="Robotic arm moving after receiving cyclic torque command " class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Robotic arm moving after receiving cyclic torque command 
</div>



Some of the results of the experiments performed can be found below:


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/pos1.png" title="Position and rotation of each motors" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Position and rotation of each motors
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/pos2.png" title="Position and rotation of each motors2" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Position and rotation of each motors
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/pos3.png" title=" Connectors PR2 Driver" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Connectors PR2 Driver
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/pos4.png" title="EVEREST NET 30/80" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    EVEREST NET 30/80
</div>




Full implementation can be found [here](https://github.com/stevedanomodolor/Simulation-and-control-of-BLDC-motor-with-methods-on-data-transfer-and-visualization) 