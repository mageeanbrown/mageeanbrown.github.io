---
layout: page
title: Bio-inspired Fluid Dynamics
description: Studying the hydrodynamics of an underwater robot with a shrimp-inspired design
img: assets/img/4.jpg
importance: 1
category: work
related_publications: false
---

This is a project that I worked on in the Wilhelmus Lab at Brown University. I wrote my honors thesis in mechanical engineering about this project. I also presented this project at the APS DFD conference in 2023, and my abstract gives a good overview of what the project entailed:

"Shrimp can adapt to their environment through dynamic morphology, contributing to their remarkable maneuverability and efficiency during swimming. Integral to this morphological adaptability of shrimp is the cupping of leg appendages (pleopods) during their power and recovery stroke. Cupping occurs through the change in the cupping angle between each endopodite and exopodite pair that make up a pleopod. This cupping angle contributes to the actuation of the exopodite to spread outward (abduction) during the power stroke and to move inward (adduction) during the recovery stroke. Previous studies have given insight into these pleopod kinematics. However, the optimal angle of pleopod cupping for different swimming modes and hydrodynamic conditions still needs to be explored. Here, we use biological studies of shrimp to guide the design of a robotic pleopod, which we leveraged to investigate the hydrodynamics of pleopod cupping. Through Particle Image Velocimetry (PIV) experiments and force measurements, we examine the thrust, lift, and vortex generation across a range of cupping angle configurations. We compare the cupping angle of optimal efficiency to the cupping angle found in shrimp (approximately 35°) to understand the trade-off between lift and thrust generation. Implementing the optimal cupping angle will ensure the maneuverability of future underwater metachronal robots under different environmental conditions."

Anyway, here are some fun photos/figures from the research process!

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/methods.png" title="cupping angle depiction" class="row-img rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid path="assets/img/exploded_view.jpg" title="bearing exploded view" class="row-img rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, an illustration of the pleopod model, with the relevant angles and swimming cycle phases indicated. On the right, an exploded view of the pleopod model's joint. There is a bearing to allow for smooth rotation while transitioning to/from the power and recovery strokes.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/force_transducer.jpg" title="Force transducer" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/small_tank.jpg" title="During PIV" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/particles.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the force transducer used to approximate the forces on the model synchronously with PIV data collection. The force transducer has a resolution of 1/320 N. In the middle, a view of the first experimental setup (eventually the tank size was increased) using particle image velocimetry (PIV). On the right, a closer view of the particles used during PIV. These particles are illuminated with a laser and tracked using a cross-correlation algorithm during analysis of video taken during experiments.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/vorticity_fields.png" title="vorticity fields" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A figure of analyzed PIV data at a cupping angle (zeta) of 35 degrees, showing the points of maximum thrust (left) and lift (right) throughout a stroke cycle. The color bar shows the magnitude of vorticity, and streamlines are also plotted. There are coherent leading-edge vortices (LEVs) that enhance lift generation.
</div>



