---
layout: page
title: Ball-Launcher-Reinforcement-Learning
description: A robot that learns to play basketball by using Reinforcement Learning
img: assets/img/robot_learning.png
importance: 1
category: general
related_publications: true
---

In this project, we are implementing a tossing ball robot that
learns by means of Reinforcement Learning. The robot is able
to determine its optimal actions by using Computer Vision techniques, combined with different solutions, such as Q-learning and
DDPG+HER, which have been broadly researched to have a higher
accuracy. Simulations have also been done with OpenAI Gym and
ROS (Gazebo), prior to the real implementation, to deeply study
the best approach and prepare the model for the real scenario{% cite robot_learning %}.

The following vide shows the reesult of the project: 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/a_robot_that_learns_to_play_basketball_by_using_reinforcement_learning (1080p).mp4" title="example image" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Ball-Launcher-Reinforcement-Learning
</div>



Some of the results of the experiments performed can be found below:


<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/train1.png" title="Training result using Q-learning" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Training result using Q-learning Simulation
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


# Conclusions 
In this report, a robot is taught to toss a ball into a bucket using reinforcement
different reinforcement learning techniques. In order to do so, a prototype has
to be built from scratch both in the real world and in simulation.
Despite the limited robustness of the robot, the results presented before
are quite promising, both in simulation and in the real-scenario. Using DDPG
with HER is a good choice for this kind of application where you need trial
and error experiments, and its success rate was good and fast. Adding HER is
very useful when the states are varying and the model learns faster.
There are some variations that ought to be made to enhance the perfor-
mance, however, the designed first prototype has a huge potential.

Full implementation can be found [here](https://github.com/stevedanomodolor/robot_learning) 