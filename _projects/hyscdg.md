---
layout: page
title: The Change You Want To Detect
description: Semantic Change Detection In Earth Observation With Hybrid Data Generation
img: assets/img/teaser.png
importance: 1
category: work
related_publications: true
images:
    compare: true
    slider: true
---

Semantic Change Detection (SCD) in remote sensing comes with its fair share of challenges. Especially when tackling the task on very high resolution pairs of aerial images.
Pixel-level annotated Semantic Change datasets as HRSCD [{% cite hrscd %}], SECOND [{% cite second %}] or HiUCD [{% cite hiucd %}] exists but each comes with its drawbacks. Lack of diversity, scarce and coarse annotations, limited resolution, etc.  
Training large deep learning models on these data is possible, but doesn't offer any generalization capacity. Annotating large set of data would require giant amount of time.
In such a context, simulation and especially synthetic data generation appears as a really good solution to mitigate these difficulties. 


### **FSC-180k** : A large-scale hybrid dataset for very high resolution semantic change detection

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img-comparison-slider>
          {% include figure.liquid path="assets/img/IMG2.jpg" class="img-fluid rounded z-depth-1" slot="first" %}
          {% include figure.liquid path="assets/img/IMG1.jpg" class="img-fluid rounded z-depth-1" slot="second" %}
        </img-comparison-slider>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img-comparison-slider>
          {% include figure.liquid path="assets/img/IMG2.jpg" class="img-fluid rounded z-depth-1" slot="first" %}
          {% include figure.liquid path="assets/img/IMG1.jpg" class="img-fluid rounded z-depth-1" slot="second" %}
        </img-comparison-slider>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img-comparison-slider>
          {% include figure.liquid path="assets/img/fsc/053420_0.png" class="img-fluid rounded z-depth-1" slot="first" %}
          {% include figure.liquid path="assets/img/fsc/053420_1.png" class="img-fluid rounded z-depth-1" slot="second" %}
        </img-comparison-slider>
    </div>
</div>
<div class="caption">
    Samples of images pairs from our **FSC-180k** dataset. Left image is generated from the original image (on the right) by our **HySCDG** pipeline.
</div>

### What we propose : hybrid data generation and efficient transfer learning
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/teaser.png" title="The whole process" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
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
