---
layout: page
title: Bio-inspired Robotics and Fluid Dynamics
description: Studying the hydrodynamics of an underwater robot with a shrimp-inspired design
img: assets/img/4.jpg
importance: 1
category: engineering
related_publications: 
  - brown_analysis_2023
  - oliveira_pedro_dos_santos_exploring_nodate
---

This is a project that I worked on in the Wilhelmus Lab at Brown University. I wrote my honors thesis in mechanical engineering about this project. I also presented this project at the American Physical Society Division of Fluid Dynamics (APS DFD) conference in 2023, and my abstract gives a good overview of what the project entailed:

"Shrimp can adapt to their environment through dynamic morphology, contributing to their remarkable maneuverability and efficiency during swimming. Integral to this morphological adaptability of shrimp is the cupping of leg appendages (pleopods) during their power and recovery stroke. Cupping occurs through the change in the cupping angle between each endopodite and exopodite pair that make up a pleopod. This cupping angle contributes to the actuation of the exopodite to spread outward (abduction) during the power stroke and to move inward (adduction) during the recovery stroke. Previous studies have given insight into these pleopod kinematics. However, the optimal angle of pleopod cupping for different swimming modes and hydrodynamic conditions still needs to be explored. Here, we use biological studies of shrimp to guide the design of a robotic pleopod, which we leveraged to investigate the hydrodynamics of pleopod cupping. Through particle image velocimetry (PIV) experiments and force measurements, we examine the thrust, lift, and vortex generation across a range of cupping angle configurations. We compare the cupping angle of optimal efficiency to the cupping angle found in shrimp (approximately 35°) to understand the trade-off between lift and thrust generation. Implementing the optimal cupping angle will ensure the maneuverability of future underwater metachronal robots under different environmental conditions."

Below are some CAD renderings (made using Fusion 360) of the robotic pleopod, with the relevant angles denoted. 

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/methods.png" title="cupping angle depiction" class="row-img rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid path="assets/img/exploded_view.jpg" title="bearing exploded view" class="row-img rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, a rendering of the pleopod model, with the relevant angles and swimming cycle phases indicated. On the right, an exploded view of the pleopod model's joint. There is a bearing to allow for smooth rotation while transitioning to/from the power and recovery strokes.
</div>

Designing the exopodite was an unexpected challenge. Since the entire model was mounted sideways in the tank, I needed the exopodite to be precisely neutrally buoyant to ensure that passive acuation could occur. I originally used an FDM 3D printer to fabricate the exopodite, and I attempted to tune the infill of the model to achieve the correct buoyancy. However, with a model this small, it was not possible to consistently achieve that same buoyancy at one infill setting. I discovered that the tolerance of the 3D printer was too large for the precision I was trying to achieve. Because of this, I switched to SLA 3D printing, which typically offers better resolution than FDM. However, I again encountered the same issue, where the 3D printer tolerance was too large to achieve consistent buoyancy given the same slicing settings. 

To solve this issue, I designed the exopodite with an internal pocket, which meant that uncured resin would pool up inside the model during printing. After the printing process, I would make a small hole with a needle and iteratively drain resin from the model until the buoyancy was correct. Upon reaching the correct buoyancy, I sealed the small hole and did a complete curing cycle to prevent movement of resin in the model. This also allowed me to choose where the center of buoyancy was located, which I located as close to the mounting joint (near the bearing) as possible, which mitigated the effect of buoyancy on the orientation of the exopodite. In the CAD images below, you can see the cross-section of the exopodite with the internal pocket.

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/full_exo.png" title="" class="row-img rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid path="assets/img/sliced_exo.png" title="" class="row-img rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, an image of the CAD model of the exopodite. The dovetail on the mounting end allows the cupping-angle joints to be swapped without having to manufacture a new exopodite for every trial. On the right, a section view of the exopodite with the internal pocket visible. Once the buoyancy was tuned, the pocket would be mostly filled with resin, with some resin removed from the region of the pocket closest to the mounting joint.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/force_transducer.jpg" title="" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/small_tank.jpg" title="" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/particles.jpg" title="" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the force transducer used to approximate the forces on the model synchronously with PIV data collection. The force transducer has a resolution of 1/320 N. In the middle, a view of the first experimental setup (eventually the tank size was increased) using particle image velocimetry (PIV). On the right, a closer view of the particles used during PIV. These particles are illuminated with a laser and tracked using a cross-correlation algorithm during analysis of video taken during experiments.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/vorticity_fields.png" title="" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A figure of analyzed PIV data at a cupping angle (zeta) of 35 degrees, showing the points of maximum thrust (left) and lift (right) throughout a stroke cycle. The color bar shows the magnitude of vorticity, and streamlines are also plotted. There are coherent leading-edge vortices (LEVs) that enhance lift generation.
</div>


If you are interested in reading my full honors thesis, it is available below:
<!-- PDF Preview -->
<div class="row mt-5">
  <div class="col-12">
    <h3 class="mb-3">Undergrad Honors Thesis</h3>
    <embed 
      src="{{ '/assets/pdf/Honors_Thesis_Archive.pdf' | relative_url }}" 
      type="application/pdf" 
      width="100%" 
      height="800px"
      style="border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);" />
    <p class="mt-3 text-center">
      <a href="{{ '/assets/pdf/Honors_Thesis_Archive.pdf' | relative_url }}" target="_blank" class="btn btn-primary">
        Open / Download PDF
      </a>
    </p>
  </div>
</div>


