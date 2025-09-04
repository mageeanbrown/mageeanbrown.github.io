---
layout: page
title: Bicycle Frame Building
description: Designing and fabricating a bicycle frame from scratch
img: assets/img/frame_jig.jpg
importance: 3
category: engineering
related_publications: false
---

This project evolved from an independent study project that I started during one semester of undergrad. At the time that I began the project, I had barely used CAD, had very little machining experience, and was just beginning to seriously practice TIG welding. Unsuprisingly, building a bicycle frame from scratch required that I get good at all of these skills. 

By the end of that first semester, I got very comfortable with CAD and taught myself how to run FEA in Solidworks. Below are some images of my main CAD drawing and some FEA. 

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/cad_file.png" title="cad file" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/fea_frame.png" title="fea" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the bike dimensions are designed using SolidWorks. On the right, FEA results (again using Solidworks) that I simulated during my independent study.
</div>

I also improved my machine shop skills throughout this project, racking up many hours on the manual mills and lathes, as well as on the CNC mill. But alas, during my original attempt at the project, my welding skills were not honed enough to weld the thin bicycle tubing (some tubes are as thin as 0.028 inches!). 

A year later, and after welding a racecar (see more about this [here](/projects/2_project/)), I returned to the project with much more fabrication experience. I designed and machined a high-precision and adjustable jig, which is essential for holding all the components tightly together during the welding process. Then, after getting the tubes cut according to my CAD design, I was able to weld the frame fully. I also brazed for the first time to attach some of the smaller components, like the water bottle bosses.

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/machining.jpg" title="machining the jig" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/chainstays.jpg" title="cutting tubes" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, machining a part for the jig on the mill. Precision was critical for this project, so I kept all tolerances within 0.002 inches. On the right, an image taken mid-way through coping the chainstays. These were tricky tubes to cope because they are bent, have a non-uniform cross-section along the length, and need to be cut at compound angles. The paper that you see wrapped on one end of the tube was extremely helpful during this cutting process. After creating flattened drawings of the tubes in SolidWorks (you can see some of the original drawings on the table in this image), I printed out these guides to show me where the cuts needed to be made. 
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/jig1.jpg" title="jig in progress" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/jig2.jpg" title="jig in action" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    The jig in action. Creating the jig took much longer than the actual welding process, but is essential for achieving precise frame geometry and making strong welds. The components I machined to hold the tubes are made from aluminum and are mounted on a T-slot aluminum extrusion, allowing the entire system to be adjustable for future frames.
</div>

Below, you'll see some of my more recent welds (getting better, but still more practice to be done!) and the frame post-welding/brazing. The final steps will involve painting the frame, facing and reaming the frame (to remove distortion from welding in important areas, such as the bottom bracket shell, head tube, and seat tube), and buying/installing the remaining parts to make the bike ready for riding.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/welding_improvements.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/finished_frame.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    My welding progress on the left and the fully welded frame on the right.
</div>
