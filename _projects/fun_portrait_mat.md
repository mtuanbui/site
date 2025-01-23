---
layout: page
title: fast portrait matting for web browsers
description: MODNet inference in a web browser
# img: assets/img/projects/bgremover_bg.png
importance: 1
category: fun
related_publications: false
---

In 2022, while searching for real-time solutions to remove backgrounds from portrait photos, I stumbled upon the GitHub repository for [MODNet](https://github.com/ZHKKKe/MODNet). Impressed by the results of the technical paper, I decided to undertake a small project to make MODNet run in a web browser. I used the Tensorflow.js library and WASM for this small project. Most of the work was quite simple except for converting the pretrained model to a format compatible with Tensorflow.js, which took more time than expected.

I also developed a basic web application for the project. The user interface allows users to select a portrait photo from a provided list or upload a new one. Background removal is initiated by clicking the `Remove Background` button. MODNet model inference runs fast and entirely locally thanks to Tensorflow.js, which utilizes WebGL acceleration at its core.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/bgremover_ui.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <a href="https://mtuan4i.github.io/BackgroundRemover/">mtuan4i.github.io/BackgroundRemover</a>
</div>

