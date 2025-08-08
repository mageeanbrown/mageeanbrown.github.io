---
layout: page
title: Wearable Hand Tremor Attenuator
description: Developing a wrist-watch-like electromechanical device to actively reduce hand tremors.
img: assets/img/TRUhold.jpg
importance: 2
category: work
giscus_comments: false
---

This was my senior capstone project during undergrad. I worked with a group of 5 friends to design and prototype a wearable device that can reduce hand tremors, specifically targeting Parkinson's disease patients. Throughout this project, we had conversations with over 20 medical professionals to determine what design features would be the most valuable for their patients. Eventually, we decided upon a design that uses the principle of destructive interference of waves. Since tremors cause the hand to move in approximately a sinusoidal pattern, our system utilizes a controllable mass that moves at a 180-degree phase offset from the tremor itself. Two back-to-back solenoids were used to control the movement of the mass (in this case, the mass is a magnet core), and we used feedback from an accelerometer to infer the frequency and phase of the tremor.

Since we were unable to test our device on actual patients (the process of getting approval for this could not be completed in a semester), we created a tremor simulator using an eccentric mass attached to a small motor, which could also be worn on the wrist. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rubber_test.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/arm_test.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Testing our tremor simulator (in black housing) on an artificial (left) and actual arm (right). The accelerometer is attached to the arm/hand in both images to measure the simulated tremor frequency.
</div>

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/circuitDiagramSolenoidControl.jpg" title="Circuit diagram" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/full_device.jpg" title="Tremor device" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the right, a circuit diagram of our device. On the right, the tremor attenuator (white housing), accelerometer, and tremor simulator (black housing) on a hand. 
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/FinalFinal5Hz.jpg" title="5 Hz data" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/FinalFinal6Hz.jpg" title="6 Hz data" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Accelerometer data from testing the device at 5 Hz and 6 Hz. In all cases, there was a significant reduction in tremor amplitude with the device on. For future iterations of the design, we plan to better tune the PID control system to improve attenuation.
</div>


Reducing the overall size of the device not something we had time for during the semester, but we understand is an important consideration for patients. Because of this, we created a "looks-like" prototype. The prototype is designed based on the dimensions of a piezoelectric micro linear actuator we would like to use in the future (it was beyond our current budget), as well as a standard battery pack that would allow the device to function all day without charging. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/looks_like_prototype.jpg" title="looks-like prototype" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/looks_like_arm.jpg" title="looks-like prototype on arm" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The "looks-like" prototype of our device. The device uses a rechargable battery pack with a large enough capacity to work all day.
</div>

