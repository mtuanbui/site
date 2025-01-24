---
layout: page
title: Detect and refine margin lines on a 3D tooth model
description: a geometry processing project that I researched and developed while being a research student in Computer Graphics
img: assets/img/projects/dental_bg.png
importance: 5
category: work
related_publications: false
---

The image below illustrates the margin line in dental restorations.

> A margin line is the boundary between the natural tooth structure and the artificial restorative material.
> It is the visible edge where the filling, crown, or other restoration meets the original tooth.

<div class="row">
    <div class="mx-auto col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/dental_bg.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

During my time as a research student, I undertook a research project to develop an algorithm for detecting margin lines in input 3D tooth models. I successfully developed a semi-automatic solution that enables the detection of smooth margin lines with only one input anchor point. Additionally, I proposed a method to refine the detected margin line by either selecting points or sketching along the correct margin line. The algorithms operate reliably and provide near-instantaneous feedback, as demonstrated in the videos below.

<div class="row">
    <div class="mx-auto col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/singlepoint_margin.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Single-point margin line detection
</div>

<div class="row">
    <div class="mx-auto col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/click_margin.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Point-based margin line refinement
</div>

<div class="row">
    <div class="mx-auto col-sm-8 mt-3 mt-md-0">
        {% include video.liquid path="assets/video/sketch_margin.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
<div class="caption">
    Sketch-based margin line refinement
</div>
