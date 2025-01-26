---
layout: page
title: Real-time HDR lighting environment map estimation
description: lightweight deep neural network for real-time estimating a HDR lighting environment map from a single LDR input image
img: assets/img/projects/envmap_bg.png
importance: 2
category: work
related_publications: false
---

This project extends [DeepLight](https://arxiv.org/abs/1904.01175) by exploring synthetic data for model training. Unlike the original work, which required a custom-built device for data collection, our approach leverages synthetic datasets, significantly reducing data acquisition costs. Furthermore, instead of training a model to predict mirror ball maps as in DeepLight, our model directly predicts HDR equirectangular lighting environment maps.

In essence, I developed a compact deep learning model capable of estimating a High Dynamic Range (HDR) lighting environment map from a single Low Dynamic Range (LDR) RGB image. The model's speed allows it to process video frames from a live mobile camera in real time.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/envmap_predict.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An example of the input LDR image, equirectangular HDR lightning map predicted by our model and the ground-truth
</div>

The primary application of the model is to render 3D models consistently with a background image. This is accomplished by utilizing the HDR lighting map, predicted by the model from the input background image, to illuminate the 3D models. The following image demonstrates the model's application with a variety of input backgrounds.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/envmap_results.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Virtual objects were illuminated using the HDR map predicted by the model, which takes the background image as input.
</div>

Finally, the clip below demonstrates how the model processes video frames.

<div class="row">
    <div class="mx-auto mt-3 mt-md-0">
        {% include video.liquid path="assets/video/envmap_video.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=false %}
    </div>
</div>
