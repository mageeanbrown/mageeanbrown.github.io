---
layout: page
title: Brown Formula Racing Subsystems
description: Leading the design and fabrication of the chassis and steering subsystems
img: assets/img/table_welding.jpg
importance: 2
category: engineering
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
    <div class="col-sm-9 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/iteration_of_chass.png" title="chassis iterations" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An example of the iteration process that occurs during the design and simulation phase of the project. Typically, there is a trade-off between high torsional stiffness and weight, so we optimize these variables to get a light but stiff chassis.
</div>

Once the design is complete and our team has passed SES (structural equivalency spreadsheet; this ensures important rules are met), we order our tubes, which are laser-cut out of house. While we wait on the tubes to arrive, we manufacture jigs so the tubes can be properly held in place while we weld. This can be a pretty tricky process, but without good jigs, the welding process is hopeless. For our jigs, we machine posts that hold all of our suspension hardpoints, which in turn hold our chassis tubes together. For areas a bit farther from the heat-affected zone, we add 3D printed jigs to confirm that everything stays in the correct place.

<div class="row">
    <div class="col-sm-9 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/jig_horizontal.jpg" title="chassis iterations" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
The jigging process for the rear bay. Here, we use a jigging engine in addition to the machined posts, which has all the same mounting points as the actual engine. For the machined posts, most of the material is aluminum for ease of machining; however, the angle mounts that bolt onto the chassis hardpoints are steel. Using steel for these pieces ensures that the jig will not deform before making the weld, since aluminum has a lower melting point than steel.
</div>

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
    On the left, the finished 2024 car, "Rhode Rage". On the right, the car at the Formula SAE Michigan competition.
</div>


Steering Subsystem (2023):

For the steering subsystem, I implemented a relatively simple rack-and-pinion steering design. During the design process, I chose to optimize handling and ergonomics, while minimizing weight, compliance, and steering effort. Because of this, I had to collaborate heavily with the suspension and ergonomics subsystems, and gained valuable experience working with teammates with different areas of expertise. 

Here are some CAD images of the steering system, which I will explain in more detail below.

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/steering_top.png" title="steering system side" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/steering_side.png" title="steering system top" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the steering system modeled in SolidWorks. On the right, a side view of the steering system in the car. The plane visible in this CAD image is tangent to the top of the front roll bar. The entire steering system must be below this plane (even with the steering wheel completely turned, as in the image) to ensure that the driver's hands are protected by the chassis if the car were to crash.
</div>

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/steering_rack.jpg" title="steering rack" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/rack_mount.png" title="rack mount" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, an image of the steering rack, which is the NARRCO 17.4” eye-to-eye, with a 3.46 in/rev rack speed and 13.4-tooth pinion. On the right, a CAD image of one of the mounts that holds the rack in place. These mounts are machined from steel, and one side of the mount is welded to the chassis.
</div>

This design had 98% static positive geometry to optimize slip angle at relatively low speeds in a tight FSAE corner radius. The system also had 82% dynamic Ackermann at minimum turning radii. A similar number was found for the very small turning radius of 1 wheelbase (~63 inches). A 280 degree lock-lock steering wheel range allows for comfortable steering effort and ergonomics, and the car has an approximately 4:1 steering ratio.

Below are images of some of the FEA that I ran on the upper steering mount, steering shaft, and bearing housing. For these parts, it is primarily torque and lateral forces from the driver applied at the steering wheel that are important to consider. 

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/fea_mount.jpg" title="FEA of steering mount" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/shaft_fea.png" title="FEA of upper shaft" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/fea_bearing.png" title="FEA of bearing housing" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
   On the left, FEA of the steering mount, which is one of the points of attachment between the steering system and chassis. In the middle, FEA of the upper shaft is shown. The primary hole shown is for electrical wires to exit. On the right, FEA of the bearing housing, which holds the steering shaft and allows the entire column to rotate smoothly when the driver turns. In all of these images, magenta arrows indicate force vectors, while green arrows are constrained points. In the bearing housing image, there are no arrows visible, but this analysis was run with lateral forcing applied and constraints at the mounting points. Based on literature values, 660 N of force and/or 150 Nm of torque is applied throughout the analyses.
</div>

For the fabrication stage of the project, I machined and/or welded all components, aside from the steering rack and steering wheel quick-release, which we purchased off-the-shelf. Here are some images of the different parts, as well as the assembled system!

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/mount_before.png" title="pre-welding steering mount" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/mount_after.png" title="steering mount welded on car" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the steering system mount before welding. This mount is made from steel and the pieces are laser cut out-of-house (it is designed with cut-outs for weight reduction, rather than having full steel sheets that provide a similar strength). On the right, the mount after I welded it to the car. This was my first welded part that made its way onto the car!
</div>

<div class="row align-items-center custom-row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/assembly.jpg" title="steering assembly" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/driving_day.jpg" title="driving day" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the assembly of the bearing housing, upper shaft, and spline are visible. The steering wheel attaches to the spline and can be removed for quick driver egress. On the right, the almost complete car on one of our driving days, where we collect data and make adjustments before the competition in May.
</div>
