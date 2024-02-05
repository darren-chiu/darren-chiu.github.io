---
layout: page
title: Miura-Bot, Self Folding Robots
description: Can we use the Miura-Ori pattern as a form of locomotion or self-assembly?
img: assets/img/miura_cell.jpg
importance: 1
category: robots
related_publications: false
---
Designs for my final project in CEE345, Origami Engineering, at Princeton. A robot that mimics the miura-ori pattern for self folding and mobility. Each parallelogram in a miura unit cell would comprise of two custom PCBs, four motors, and interlocking mechanisms for self folding and self assembly. Each robot runs off a single rechargeable 3.3V battery that powers the motors and all electronics. 

Programming the board using a USB-TTL board, we found that unfortunately, the first iteration of this board could not drive motors as I forgot to place bypass capacitors on the motor controllers. In parallel, the software was developed for flat locomotion using a protoboard and preliminary chasis. 

The second iteration of the board is an improved design with 4 layers and 2 sides of componenets. This board has a reduced size and can drive up to six motors after the bypass capacitors were placed. 

After soldering together components of the board, the initial design is now complete. We control all indiviudal unit cells using an esp32 over a web server on the host laptop. Quick demo code was written to fold the robot from a flat configuration into the folder miura-ori pattern. Below is an actuation of each individual panel. 

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/miura_folding_individual.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/miura_fold.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Folding Miura Bot
</div>

Improved versions were created with the ability to self assemble and fold. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/miura_self_assembly.gif" title="Miura Bot Class Poster" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Self Assembling Prototype
</div>

Below is the poster presentation of our completed project describing the mechanical and electrical design. Future work is currently being discussed for improved designs and potential formal publication.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/miura_poster.jpg" title="Miura Bot Class Poster" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Miura Bot Class Poster
</div>
