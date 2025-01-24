---
layout: page
title: Real-time rigid deformation for web browsers
description: an implementation of Image Deformation Using Moving Least Squares for web browser
# img: assets/img/projects/imgwarp_bg.png
importance: 2
category: fun
related_publications: false
---

While exploring WebAssembly (abbreviated WASM), I attempted to port the [Image Deformation Using Moving Least Squares](https://dl.acm.org/doi/10.1145/1141911.1141920) algorithm to the web environment. I re-implemented the algorithm in the paper using C++, then used Emscripten to build the C++ code into WASM format that can be loaded and used by the webpage's JavaScript code.

The web user interface allows users to select an input image from a list or upload a new one. To deform the input image, you can move the control points by clicking and dragging them. Thanks to the efficiency of the algorithm and WASM, the image will be warped and updated almost immediately as the control points are moved. Additionally, you can add/remove control points as well as switch between Affine/Rigid deformation.

<div class="row">
    <div class="col-sm mt-3 mt-md-0"></div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/imgwarp_ui.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0"></div>
</div>
<div class="caption">
    <a href="https://mtuan4i.github.io/ImageWarping">mtuan4i.github.io/ImageWarping</a>
</div>
