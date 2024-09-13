---
layout: page
title: Multirobot control
description: Algorithms for controlling multiple robot including Agv and Uav at the same time. 
img: assets/img/projects/communication_architecture.png
importance: 1
category: work
related_publications: true
---

Although there has been advancement in drone (UAV) technology 
{% cite Omodolor_2022 %}, issues like flight duration, computation load and mission complexity still limit usage of the full potential of this technology. In this thesis, this problem is tackled using multiple drones and mobile robots(UGV).

Nowadays, drone missions are becoming complex and drones are used for
long-range missions. This has resulted in the need for strategies that can leverage the current limitation of this technology, while performing these missions
and satisfying energy and time constraints. Imagine if, instead of one drone
performing a surveillance mission, we have two or more. We can cover larger
areas faster. Now, consider long-range surveillance missions. One downside of
drones is their limited battery life. Constantly returning them to a home base
might waste mission time. In addition, installing multiple charging stations
along the drone path is expensive, time-consuming and in most cases impossible because of the mission topology. In this situation, by combining mobile
robots and drones, we get the benefits of both worlds. Mobile robots can carry
more weight and have longer battery lives, while drones can perform more
complex maneuvers.

This thesis tries to solve the following problem: how do we coordinate fleets
of drones and fleets of mobile robots while avoiding collisions with obstacles.
The investigated approach considers two aspects: how to maintain the desired
formation between the drones and how to coordinate the drones and the mobile
robot. In the first case, a potential-based approach similar to how animals
flock in nature is used to maintain the desired shape between the drones. One
way to understand the idea of potential is to assume they are the tension
applied to a spring that connects the robots, see Fig. 1. The goal is to arrive
at a configuration where no tensions exist in the springs. In the second case, a 
cluster-based leadership-follower approach algorithm is used where the mobile
robot has to follow clusters of the drones.


An essential aspect of the approach used is that it does not depend on a
central planning and control system and it is intended to run on computationally constrained hardware. In addition, the number of drones can be modified even after reaching the desired formation shape. This is quite useful, especially
when the use case requires flexibility, like when one drone in the formation might have to land on the mobile robot for recharging without affecting the other drones in the formation shape. The developed approaches were implemented and evaluated both in simulations and in experiments on hardware. 
Video demonstrations can be found in the [link](https://www.youtube.com/playlist?list=PLdsouUoVwMKNFyUv798AElfGWj3b5Zl1F)

The following videos are some of the results of the thesis. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/multirobot_control.mp4" title="example image" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Free-space 3 UAV and 1 UGV formation and flocking control
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/Three UAV formation and flocking with obstacle(dynamic) avoidance.mp4" title="example image" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Three UAV formation and flocking with obstacle(dynamic) avoidance
</div>

Some of the results of the experiments performed: can be found below:
Free-space UAV Formation and Orientation:


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/num1_real.png" title="free-space UAV Formation and Orientation" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/num2_real.png" title="Free-space UAV Formation and Flocking" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure on the left shows the free-space UAV Formation and Orientation while figure on the right shows  Free-space UAV Formation and Flocking
</div>


<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/num3_real.png" title="three UAVs for free-space formation and flocking
with obstacle avoidance" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/num4_real.png" title="Free-space UAV Formation and Flocking" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Figure on the left shows the three UAVs for free-space formation and flocking
with obstacle avoidance  while figure on the right shows  Free-space UAV Formation and Flocking
</div>

Full implementation can be found [here](https://github.com/stevedanomodolor/formation_and_coordination_of_UAV_and_UGV) 