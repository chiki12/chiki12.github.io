---
layout: page
title: Bachelor Thesis (202503)
description: Prompt Optimization for Outfit Generation through Neural Network-based Feedback Loops
img: assets/img/thesis/1.jpg
importance: 1
category: research
related_publications: false
---

## Title: Prompt Optimization for Outfit Generation through Neural Network-based Feedback Loops
#### Undergraduate Thesis 
#### Graduation date: March, 2025
#### Advisor: Professor Katsuki Fujisawa

For undergraduate thesis, we proposed a workflow of automated prompt refinement for fashion image generation using language models, with the objective of utilizing the existing AI generation tools with reasonable computational cost.
By assuming compatible scores represent the unique fashion style of the dataset that the score model trained on, we use it as metric for the refinement process.

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis/1.jpg" title="Proposed Workflow" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

<div class="caption">
    The workflow of the proposed prompt refinement system, consisting of an image generator, an language model, and OutfitTransformer CP model.
</div>


By intergrating fashion scoring model{% cite sarkar2023outfittransformer %}, image generative model and large language model in the system and automize it with outfit set data, it can automatically refining the text description prompt from initial description and generate new images following scores of fashion scoring system as a sole metric.


<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/thesis/2.jpg" title="score visualization" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Scores across refinement process of the proposed system.
</div>

By utilizing fashion scoring model, image generative model and large language model, the proposed prompt refinement system achieve 70% rate of cases that got higher score than initial prompt, and 50% of the cases got higher final score than score of original images. While challenges like score flctuation, balance of prompt length, category mismatch, and unreliable score metric still remained to be addressed in the future.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/thesis/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example of a refinement process of an item. The first picture is the original image from the dataset, as the rest are generated images based on the original or refined description that is shown below the images.
</div>

