---
layout: page
title: Rovables Bayesian Inspection
description: Enabling small-scale robots to climb and inspect surfaces.
img: assets/img/rovable_tof.jpg
importance: 1
category: robots
related_publications: false
---
Simulated experiments exploring a randomized grid of black and white squares on the left. The robots are communicating with eachother as they observe the square they are on --  making decisions on if the environment is mostly black or white.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/rov_sim.gif" title="Rovables Simulation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Webots Simulation of Rovables Inspection
</div>

After simulating the rovables within Webots, hardware experiments were conducted to explore a vibrating metallic surface. Vibration motors were placed under the arena for the IMU to sense. Additionally, robot locations were tracked using OpenCV for coverage assessment and using an NRF radio to asses posterior decisions. 

As part of my Princeton senior thesis I fabricated a swarm of 20 Rovables robots and helping in the design of a 3D test bed for verification of future new inspection algorithms.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/rovables_swarm.jpg" title="Rovables Swarm" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Swarm of Rovables
</div>

Below is a 3D render of a time of flight board expansion of the individual sensor modules and the expansion that that would connect on the top of the design. Then the assembled version attached to the top of the previously designed robot. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/tof_top.png" title="Rovables Swarm" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    3D rendering of fully assembled Rovables expansion board.
</div>
<!-- 
<img align="left" width="20%" height="30%" src="/images/tof_board_individual.PNG">
<img align="right" width="80%" src="/images/tof_top.PNG">  -->

## PSO for Bayesian Inspection Algorithm
Using Particle Swarm Optimization (PSO) deployed on AWS for multi parameter heuristic optimization of the "Bayes-Bot" surface inspection algorithm. Achieved through simulation using the Webots simulation platform.
