---
layout: page
title: Brown Formula Racing Subsystems
description: Leading the design and fabrication of the chassis and steering subsystems
img: assets/img/table_welding.jpg
importance: 2
category: work
giscus_comments: false
---

I joined the Brown Formula Racing during my sophomore year of undergrad. Each year, the team builds a racecar from scratch and then competes at the Formula SAE Michigan event in May.

This project page showcases work from two subsystems that I led on the team. During my junior year, I was the solo lead on the steering subsystem. During my senior year, I co-led the chassis subsystem along with one other member.

Chassis Subsystem (2024):

The chassis subsystem design season starts during the summer before school is back in session. We use SolidWorks for all of our design, which involves many, many weldments. Running FEA throughout the design process is critical, which we also do using SolidWorks. Generally, we optimize for high torsional stiffness and low weight. Since the chassis is such a foundational part of the car, there are many rules imposed by SAE that we must design around to build a safe car. Another important aspect of our design process is ensuring that the chassis is readily manufacturable since we do almost all of the fabrication in-house. Below are a few CAD and FEA images of the chassis, and an example of the iteration process during the design stage.

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/cad_full.png" title="CAD design" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid path="assets/img/FEA_chas.png" title="FEA" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the CAD model of the chassis. The tubes of the same color indicate the same thickness. On the right, FEA of the chassis. Here, we are trying to evaluate torsional stiffness (which is important for an effective suspension), so a force is applied upward at one of the front wheels while, on the other side, a downward force is applied. In this case, the suspension system is simply modeled as a stiff group of triangulated tubes, which allows us to isolate the chassis response to forces applied at the wheels. 
</div>

<div class="row">
    <div class="col-sm-8 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/iteration_of_chass.png" title="chassis iterations" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An example of the iteration process that occurs during the design and simulation phase of the project. Typically, there is a trade-off between high torsional stiffness and weight, so we optimize these variables to get a light but stiff chassis.
</div>

Once the design is complete and our team has passed SES (structural equivalency spreadsheet; this ensures important rules are met), we order our tubes, which are laser-cut out of house. While we wait on the tubes to arrive, we manufacture jigs so the tubes can be properly held in place while we weld. This can be a pretty tricky process, but without good jigs, the welding process is hopeless. For our jigs, we machine posts that hold all of our suspension hardpoints, which in turn hold our chassis tubes together. For areas a bit farther from the heat-affected zone, we add 3D printed jigs to confirm that everything stays in the correct place.

After the tubes are jigged, welding is then in full swing. We use tungsten inert gas (TIG) welding. This type of welding takes a lot of practice to get the hang of, which means that it is almost exclusively myself and my co-lead who weld the entire chassis, and any other parts for the car, such as the exhaust system and pedal box. 

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid path="assets/img/cj_weld.jpg" title="welding" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid path="assets/img/car_welded.jpg" title="chassis on welding table" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, some welding in action with my co-lead. This was when we had two welders running, but unfortunately, the second broke towards the beginning of the welding season. On the right, the mostly-welded chassis. Although it's a bit messy in the picture, you'll notice we have a really cool welding table! When the chassis is bolted into the jigs, which bolt into the table, we can rotate the entire table to allow for more comfortable welding positions.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/chassis_hold.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    My co-subsystem lead and I holding the chassis before sending it off to get its powder coat. The week before was spent welding almost around the clock to get the chassis done before spring classes started up.
</div>

After the chassis is welded and powder-coated, we then do physical testing on the chassis. Many of these tests are used to validate our simulations, such as those made to calculate torsional stiffness. 

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/torsion_physical_setup.jpg" title="torsion test" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/torsion_test.jpg" title="physical testing" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The physical testing setup (left) we used to validate the torsional stiffness calculated from simulations and the results (right). For the physical testup, we use machining gauges at three locations along the length of the chassis (one on each side, 6 gauges total) and measure the deflection at each point while jacking up the left front wheel of the car. From this, we were able to determine the torsional stiffness between different locations of the car, which matched up relatively well with our simulations!
</div>

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/finished_car.jpg" title="finished car" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/comp.jpg" title="competition" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the right, the finished 2024 car, "Rhode Rage". On the left, the car at the Formula SAE Michigan competition.
</div>


Steering Subsystem (2023):

While we used a relatively simple rack and pinion steering system, designing the steering geometry to properly interact with the suspension, make tight turns, and be comfortable for the driver is extremely important. Because of this, I had to collaborate heavily with the suspension and ergonomics subsystems, which was a great experience in working with other people with different areas of expertise.

Below are images of the assembly and some FEA that I ran on the upper steering shaft, which connects the steering column with the steering wheel components. I also ran many FEA simulations on the bearing housing, which helps hold the steering shaft in place while allowing rotation. For these parts, it is primarily torque and lateral forces from the driver applied at the steering wheel that are important to consider. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/steering2.jpg" title="steering mount" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/steering1.jpg" title="bearing housing and mount" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/steering_fea.jpg" title="FEA of upper shaft" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   On the left, the steering mount, which is one point of attachment between the steering system and chassis. This was one of my first car-worthy welding projects (apologies for the subpar-looking welds). In the middle, the bearing housing is the trapezoidal aluminum piece, which holds the steering shaft and allows the entire column to rotate smoothly when the driver turns. I machined this part mostly manually, except for a groove that I CNC machined for a bearing retaining ring.  The steering wheel (removable for quick  driver egress) attaches on the spline that is also in the image. On the right, FEA of the upper shaft is shown. The primary hole shown is for electrical wires to exit.
    
</div>

