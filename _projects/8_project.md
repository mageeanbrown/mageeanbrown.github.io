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
        {% include figure.liquid loading="eager" path="assets/img/FinalFinal4Hz.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/FinalFinal5Hz.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/FinalFinal6Hz.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Accelerometer data from testing the device at 4 Hz, 5 Hz, and 6 Hz. In all cases, there was a significant reduction in tremor amplitude with the device on. For future iterations of the design, we plan to tune the PID control system for better results.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
