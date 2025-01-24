---
layout: page
title: Face restoration model
description: deep neural network for fast restoration of corrupted facial images
img: assets/img/projects/facerestore_bg.png
importance: 3
category: work
related_publications: false
images:
    compare: true
    slider: true
---

In collaboration with a colleague, I undertook the development of a face restoration model inspired by [CodeFormer](https://github.com/sczhou/CodeFormer/tree/master). While CodeFormer is a widely recognized and hightly effective model, its commercial application is subject to restrictions. To address this limitation, we embarked on the creation of our own face restoration model. Although our approach shares similarities with CodeFormer's overall methodology, we implemented strategic modifications to the neural network architecture. These modifications have resulted in enhanced identity alignment of the restored faces without sacrificing image quality.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/facerestore_compare.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The image above presents a side-by-side comparison between the results of our model and CodeFormer. It can be observed that both models produce results with high fidelity. However, the faces restored by our method exhibit a higher degree of identity alignment with the ground truth.

The following images demonstrate the effectiveness of our model in restoring corrupted facial regions in portrait photographs.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        <img-comparison-slider>
            {% include figure.liquid path="assets/img/projects/facerestore_input_1.png" class="img-fluid rounded z-depth-1" slot="first" %}
            {% include figure.liquid path="assets/img/projects/facerestore_output_1.png" class="img-fluid rounded z-depth-1" slot="second" %}
        </img-comparison-slider>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img-comparison-slider>
            {% include figure.liquid path="assets/img/projects/facerestore_input_2.png" class="img-fluid rounded z-depth-1" slot="first" %}
            {% include figure.liquid path="assets/img/projects/facerestore_output_2.png" class="img-fluid rounded z-depth-1" slot="second" %}
        </img-comparison-slider>
    </div>
</div>



