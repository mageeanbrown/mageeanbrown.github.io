---
layout: page
title: Brown Formula Racing Subsystems
description: Leading the design and fabrication of the chassis and steering subsystems
img: assets/img/table_welding.jpg
importance: 2
category: work
giscus_comments: false
---

I joined the Brown Formula Racing during my sophomore year of undergrad. Each year, the team builds a racecar from scratch. The team then competes at FSAE Michigan each May, which is a competition consisting of universities across the world. 

During my junior year (2023), I was responsible for the steering system of the car. While we used a relatively simple rack and pinion steering system, designing the steering geometry to properly interact with the suspension, make tight turns, and be comfortable for the driver is extremely important. Because of this, I had to collaborate heavily with the suspension and ergonomics subsystems, which was a great experience in working with other people with different areas of expertise.

Below are images of the assembly and some FEA that I ran on the bearing housing that the upper steering shaft sits in. I also ran many FEA simulations on the joint that connects the two shaft pieces. For these parts, it is primarily torque and lateral forces from the driver applied at the steering wheel that are important to consider. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/steering2.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/steering1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/steering_fea.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   On the left, the steering mount, which is one point of attachment between the steering system and chassis. This was one of my first car-worthy welding projects (apologies for the subpar-looking welds). In the middle, the bearing housing is the trapezoidal aluminum piece, which holds the steering shaft and allows the entire column to rotate smoothly when the driver turns. I machined this part mostly manually, except for a groove that I CNC machined for a bearing retaining ring.  The steering wheel (removable for quick  driver egress) attaches on the spline that is also in the image. On the right, FEA of the bearing housing is shown. 
</div>

My senior year (2024), I became a co-lead of the chassis subsystem with one other member. This subsystem involves designing and fabricating the entire frame of the car and any other welding that subsystems require. This is also one of the first subsystems that need to be completed in the year, as every other subsystem mounts and test their parts on the chassis. Because of this, we start some of the design and simulation process by late summer so we can order our tubes (we get them coped out-of-house) and get everything jigged, and then welded by February. After welding is complete, we do physical testing to verify our simulations, such as validation of torsional stiffness estimates. 

Below are some images from the design, testing, and fabrication of the car which took place over many, many months!

<div class="row">
    <div class="col-sm-8 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/iteration_of_chass.png" title="Chassis Iterations" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An example of the iteration process that occurs during the design and simulation phase of the project. Typically, there is a trade-off between high torsional stiffness and weight, so we optimize these variables as best as we can to get a light but stiff chassis.
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
    The physical testing setup we used to validate the torsional stiffness calculated from simulations (left) and the results (right). For the physical testup, we use machining gauges at three locations along the length of the chassis (one on each side, 6 gauges total) and measure the deflection at each point while jacking up the left front wheel of the car. From this, we were able to determine the torsional stiffness between different locations of the car, which matched up relatively well with our simulations!
</div>

<div class="row">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/car_welded.jpg" title="rear bay" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/finished_car.jpg" title="finished car" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Welding progress (left) and the finished 2024 car (right), "Rhode Rage".
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/chassis_hold.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    My co-subsystem lead and I holding the chassis before sending it off to get its powder coat. The week before was spent welding almost around the clock to get the chassis done before spring classes started up.
</div>

