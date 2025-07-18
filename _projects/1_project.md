---
layout: page
title: Bicycle Framebuilding
description: Designing and fabricating a bike frame from scratch
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

This project evolved from an independent study project that I did over the course of one semester during undergrad. At the time that I began the project, I had barely used CAD, had very little machining experience, and was just beginning to seriously practice TIG welding. Unsuprisingly, building a bicycle frame from scratch required that I get good at all of these skills. 

By the end of that first semester, I could design my models with ease, and taught myself how to run FEA in Solidworks. I also got much better in the machine shop, and racked up many hours on the manual mills and lathes, as well as on the CNC mill. But alas, my welding skills were not honed enough to weld the thin bicycle tubing (some tubes are as thin as 0.028 in), so I did not complete the project that semester. 

A year later, and after welding a racecar (see more about this here), I returned to the project with much more fabrication experience. I designed machined a high-precision and adjustable jig, which is essential for holding all the components tightly together during the welding process. Then, after getting the tubes cut according to my CAD design, I was able to fully weld the frame. I also brazed for the first time to attach some of the smaller components, like the water bottle bosses.

Unfortunately, I had to leave this project at home when I moved across the country for grad school. The rest of the components still need to be assembled, but I am very proud of how the frame turned out!
    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/cad_file.png" title="cad file" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/fea_frame.png" title="fea" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/chips.jpg" title="chips" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, the bike dimensions designed using Solidworks. In the middle, FEA results (again using Solidworks) that I simulated during my independent study. On the right, machining part of the jig that I used to weld the frame.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
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
