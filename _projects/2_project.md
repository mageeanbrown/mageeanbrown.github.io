---
layout: page
title: Brown Formula Racing Subsystems
description: Leading the design and fabrication of the chassis and steering subsystems
img: assets/img/table_welding.jpg
importance: 2
category: work
giscus_comments: true
---

I joined the Brown Formula Racing during my sophomore year of undergrad. Each year, the team builds a racecar from scratch, using an internal combustion engine. The team then competes at FSAE Michigan each May, which is a competition consisting of universities across the world. 

During my first year on the team, I got a flavor of the many subsystems, starting with attaching connectors on the wiring harness, sanding composite molds, and making some simple parts in the machine shop. In my junior year (2023), after gaining some design and fabrication experience, I was put in charge of the steering system of system. While we used a relatively simple rack and pinion steering system, designing the steering geometry such that it can interact with the suspension properly, make tight turns, and be comfortable for the driver is extremely important. Because of this, I had to collaborate heavily with the suspension and ergonomics subsystems, and needed to make sure that my subsystem was fully designed and modeled in our Solidworks assembly early on. 

Below are images of the assembly and some FEA that I ran on the bearing housing that the upper steering shaft sits in. I also ran many FEA simulations on the joint that connects two shaft pieces together. For these parts, it is mostly torque and lateral forcing from the driver applied at the steering wheel that is important to look at. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rearbay.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/iteration_of_chass.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/torsion_physical_setup.jpg" title="torsion test" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/torsion_test.jpg" title="physical testing" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/chassis_hold.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    My co-subsystem lead and I holding the chassis before sending it off to get its powder coat. The week before was spent welding almost around the clock to get the chassis done before spring classes started up.
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
