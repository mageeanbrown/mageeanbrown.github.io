---
layout: page
title: High Reynolds Number Pipe Flow
description: Studying the laminar to turbulent transition in pipe flows.
img: assets/img/pipe_flow.jpg
importance: 5
category: engineering
---
This was a quarter-long project that I completed with one other classmate in my Experimental Methods class at Caltech.

Despite being ubiquitous in engineering applications, the laminar-to-turbulent transition in pipe flow still remains a significant gap in the modern understanding of fluid flows. In this project, pipe flow transition is studied experimentally, similar to Osborne Reynolds’ famous experiments in the late 19th century. These experiments gave rise to the eponymous Reynolds number, which is a nondimensional number representing the ratio of inertial effects to viscous effects. In this project, Reynolds number is defined as Re = (&#961; U D) / &#956;, where &pho is the fluid density, U is the fluid velocity, D is the pipe diameter, and &mu is the dynamic fluid viscosity.

Our setup uses a high-flow rate pump, which can produce flow rates up to 36,000 liters per hour. We pump water through a 6-foot length of glass pipe (1/4'' ID) that we got specially glassblown for the project. A diagram and image of the experimental setup are shown below.

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/exp_illus.png" title="Experimental Illustration" class="row-img rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid path="assets/img/exp_setup.jpg" title="Actual Setup" class="row-img rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, an illustration of the experimental setup. On the right, an image of the experimental setup using a 6-foot glass tube.
</div>

When the flow speeds in our pipe are increased, it is very challenging to avoid transitions from laminar to turbulent flow. This is because small disturbances are readily amplified at high Reynolds numbers. To date, the highest Reynolds number achieved in pipe flow experiments is around 100,000 (Pfenninger 1961). However, extreme precautions were made to reduce disturbances in the setup, such as conducting the experiments in a bomb shelter to minimize vibrations. One of the goals of this project was to reduce disturbances while also maintaining experimental reproducibility, since other researchers may want to conduct similar experiments elsewhere. To do this, we focused on reducing disturbances in the nozzle of the pipe, which is the transitional area between the small glass pipe and the pipe mount in the illustration above. We found that disturbances can arise from a rough surface finish and, in particular, the small lip between the nozzle and the smaller pipe section (these pieces were originally manufactured separately and then glued together). We tested several different materials for our nozzle, including plastics, precision-machined aluminum, and glass. Below, you'll see some of the qualitative testing we did to see which nozzle material and geometry was most promising.

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/nozzle_fig.png" title="different nozzles" class="row-img rounded z-depth-1" %}
</div>
<div class="caption">
Three example nozzles. Nozzles (a) and (b) were made from aluminum and grey plastic, respectively. Nozzle (b) is made from borosilicate glass, which we designed with a more gradual contraction to the uniform pipe. The glass nozzle is press-fit into the red pipe mount, which bolts into the flow conditioner. The pipe mount is 3D printed using PLA. 
</div>

<div class="container">
  <div class="row mb-3">
    <div class="col-12">
      {% include figure.liquid loading="eager" path="assets/img/al_nozzle.jpg" title="aluminum nozzle" class="img-fluid rounded z-depth-1 w-100" %}
    </div>
  </div>
  <div class="row mb-3">
    <div class="col-12">
      {% include figure.liquid loading="eager" path="assets/img/plastic_nozzle.jpg" title="plastic nozzle" class="img-fluid rounded z-depth-1 w-100" %}
    </div>
  </div>
  <div class="row mb-3">
    <div class="col-12">
      {% include figure.liquid loading="eager" path="assets/img/glass_nozzle.jpg" title="glass nozzle" class="img-fluid rounded z-depth-1 w-100" %}
    </div>
  </div>
</div>

<div class="caption">
  Images of the free jet exiting the different nozzles in the same order as in the figure above. The nozzle axis is oriented horizontally in the lab frame. The flow is from left to right, with gravity pointing down in the images. All flow rates are approximately 18.55 L/min (Re = ~46,000). The glass nozzle (bottom) has the largest laminar region in the exit jet, which indicates that it induces the least disturbances.
</div>

Another goal of this project was to develop a method for conducting particle image velocimetry (PIV) within the pipe, enabling the quantification of flow velocity and vorticity. Using standard 2D PIV methods, this is not possible because the curved surface of the glass pipe will distort the laser sheet. To mitigate this problem, we created a 'water lens', which utilizes index-of-refraction-matching so that the largest transitions in index of refraction occur at flat boundaries, normal to the laser sheet. Some images of our water lens are shown below.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/full_laser_on.jpg" title="Experimental Setup with Laser" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lens_laser.jpg" title="Water Lens" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, an image of the experimental setup with the laser on. On the right, an up-close image of the water lens with the laser sheet passing through. The water lens is made from borosilicate glass.
</div>

The rest of this page is under construction. Check back soon!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/on_priner.jpg" title="3D print" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/gled_up.jpg" title="Finished prints" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/hamer.jpg" title="Machined hammer" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/jup.jpg" title="Ski jump" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption. 
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/rickhaw.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/floers.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption. 
</div>


