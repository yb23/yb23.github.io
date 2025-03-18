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

<div class="row justify-content-center">
    <div class="col-auto">
        <h4><a href="/">Yanis Benidir</a>, <a href="#">Nicolas Gonthier</a>, <a href="">Clément Mallet</a></h4>
    </div>
</div>
<div class="row justify-content-center">
    <div class="col-auto">
        <h5 class="text-muted">LASTIG<sup>(1)</sup> - IGN<sup>(2)</sup> - ENSG<sup>(3)</sup></h5>
    </div>
</div>
<div class="row justify-content-center">
    <span class="small">(1) : Lab on Geographic Information Science for sustainable development and smart cities</span><br>
    <span class="small">(2) : Institut national de l'information géographique et forestière / French national mapping agency</span><br>
    <span class="small">(3) : École nationale des sciences géographiques</span><br>
</div>

<div class="row justify-content-center">
    <div class="col-auto">
        <a href="#" target="_blank">
        <button class="btn btn-info p-2 rounded"><i class="ai ai-arxiv" style="font-size:2em;"></i>&nbsp;&nbsp;<b style="font-size:1.5em;">Paper</b></button>
        </a>
    </div>
    <div class="col-auto">
        <a href="https://github.com/yb23/HySCDG" target="_blank">
            <button class="btn btn-info p-2 rounded"><svg class="svg-inline--fa fa-github fa-w-16" style="height:2em;" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="github" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512" data-fa-i2svg=""><path fill="currentColor" d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3.3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5.3-6.2 2.3zm44.2-1.7c-2.9.7-4.9 2.6-4.6 4.9.3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3.7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3.3 2.9 2.3 3.9 1.6 1 3.6.7 4.3-.7.7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3.7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3.7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z"></path></svg>&nbsp;&nbsp;<b style="font-size:1.5em;">Code</b></button>
        </a>
    </div>
    <div class="col-auto">
        <a href="https://huggingface.co/datasets/Yanis236/fsc-180k" target="_blank">
            <button class="btn btn-info p-2 rounded" disabled><img alt="Hugging Face's logo" style="height:2em;" src="/assets/img/huggingface_logo.svg">&nbsp;&nbsp;<b style="font-size:1.5em;">Dataset</b></button>
        </a>
    </div>
</div>

Semantic Change Detection (SCD) in remote sensing comes with its fair share of challenges. Especially when tackling the task on very high resolution pairs of aerial images.
Pixel-level annotated Semantic Change datasets as HRSCD [{% cite hrscd %}], SECOND [{% cite second %}] or HiUCD [{% cite hiucd %}] exists but each comes with its drawbacks. Lack of diversity, scarce and coarse annotations, limited resolution, etc.  
Training large deep learning models on these data is possible, but doesn't offer any generalization capacity. Annotating large set of data would require giant amount of time.
In such a context, simulation and especially synthetic data generation appears as a really good solution to mitigate these difficulties. 


### **FSC-180k** : A large-scale hybrid dataset for very high resolution semantic change detection

<div class="row justify-content-center">
    <div class="col-sm mt-3 mt-md-0">
        <img-comparison-slider>
          {% include figure.liquid path="assets/img/fsc/002292_0.png" class="img-fluid rounded z-depth-1" slot="first" %}
          {% include figure.liquid path="assets/img/fsc/002292_1.png" class="img-fluid rounded z-depth-1" slot="second" %}
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
    Samples of images pairs from our $\textbf{FSC-180k}$ dataset. Left image is generated from the original image (on the right) by our **HySCDG** pipeline.
</div>

### What we propose : hybrid data generation and efficient transfer learning
<div class="row justify-content-center">
    <div class="col-sm-8 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/teaser.png" title="The whole process" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

### Generating changes ? How it works ?
Leveraging Stable Diffusion and ControlNet through long training on VHR aerial images, we create an end-to-end "change inpainting" pipeline. Diffusion models allow to produce realistic and various textures to fulfill the original image while the control module is responsible for monitoring the semantic composition of the generated image. 
<div class="row justify-content-center">
    <div class="col-sm-8 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/pipeline.png" title="The generation pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    $\textbf{HySCDG Pipeline}$ : From a single-temporal dataset composed of one VHR image $I_1$, a semantic map $M_1$, and some openly available labeled instances, we generate a new VHR image $I_2$, a new map $M_2$ and subsequently a change map $C$.
</div>


### Transfer learning to enhance real use-cases change detection
We assess the quality of our hybrid dataset by using it in 4 transfer learning schemes : sequential, mixed, low data regime and zero-shot. Evaluation is done on 5 different real target change detection datasets.
In all cases, the performance is improved thanks to the pre-training, proof of the contribution and versatility of **FSC-180k**. We outperform scores obtained by using an other synthetic dataset, SyntheWorld.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sequential_bcd.jpg" title="Sequential Learning in Binary Change Detection" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lowdata_scd.jpg" title="Low Data Regime in Semantic Change Detection" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Results obtained by evaluating our model (pre-trained either on SyntheWorld or FSC-180k or not) through different transfer learning scenarii on real change detection datasets.
</div>


<div class="row justify-content-center">
    <div class="col-auto">
        <h6 class="text-muted">And visually...</h6>
    </div>
</div>
<div class="row justify-content-center">
    <div class="col-sm-8 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/prediction_second.jpg" title="Predictions on SECOND dataset" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Predictions obtained on SECOND either without pre-training or after pre-training on SyntheWorld or \textbf{FSC-180k} in sequential learning mode.
</div>






