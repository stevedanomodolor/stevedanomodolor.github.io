---
layout: page
title: Simulation and control of a BLDC motor
description: Simulation and control of a BLDC motor with methods on real-time data exchange and visualization.
img: assets/img/simulation.png
importance: 1
category: general
related_publications: true
---

The first objective of this thesis was to design a motor simulation web application. Despite
being a web application restricting the programming language to JavaScript, the goal was
to take advantage of the high-performance nature of a low-level language, such as C, while
maintaining the easy user interface JavaScript offered. The project also focused on finding
ways to stream the simulation result using web-based open-source software applications that
were effective and easy to implement.
After accomplishing the initial goal, the project then shifted into implementing the
motor simulation algorithms into a practical robotic application that takes into account the
multi-threaded asynchronous nature of this kind of application. When this goal was met, the
question raised was how to broadcast data from the C program to a web-based application
for visualization. From this point on, the project goes on to study a specific format that
would facilitate sending data between multiple applications independent of the programming
language and finally went into testing transport layers that would enable the data transfer.{% cite Omodolor_2020 %}.

The following user interface shows the result of the projects. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/gui.png" title="GUI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Graphical user interface showing the final simulation
</div>


 This program is based on a multithreaded application
library "Deployment Architecture model" written by members of the Robotics Research
group in Ku Leuven based on the book "Composable, adaptive, and explainable systemsof-systems" {% cite herman2017 %}. The software is made of multiples threads, activity, and algorithms. The
threads are time-triggered, meaning that they carry out loops at a specific cycle time. The
cycle continues until set false. At each iteration, the loop does one of the "4C" : composition,
communication, coordination and computation. The application uses a life-cycle state
machine to decide which of the 4c function to execute. The Life-sate cycle machines have
seven states that represent different phases of the ’lifetime’ of a thread.




<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/phase1.png" title="The different phases of the ’life-time’ of a thread" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The different phases of the ’life-time’ of a thread
</div>




<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/train2.png" title="Training results using DDPG + Sparse Reward" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Training results using DDPG Simulation
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/train3.png" title="Training results using DDPG + HER + Sparse Reward" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Training results using DDPG + HER + Sparse Reward Simulation
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/train4.png" title="Training results from the real scenario" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Training results from the real scenario
</div>




Full implementation can be found [here](https://github.com/stevedanomodolor/Simulation-and-control-of-BLDC-motor-with-methods-on-data-transfer-and-visualization) 