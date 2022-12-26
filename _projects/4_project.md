---
layout: page
title: Ice lead detection
description: Ice leads are narrow cracks in the sea-ice, which build a complex network. We worked on analyzing the dynamics of ice leads using graph neural networks.
img:  assets/img/iceleads.jpg
importance: 3
category: fun
---

An extended report for this work can be found [here](assets/../../assets/pdf/IceLeadNetworkAnalysis.pdf).
Ice lead analysis is an essential task for evaluating climate change processes in the Arctic. Ice leads are narrow cracks in the sea-ice, which build a complex network. While detecting and modeling ice leads has been performed in numerous ways based on airborne images, the dynamics of ice leads over time remain hidden and largely unexplored. These dynamics could be analyzed by interpreting the ice leads as more than just airborne images, but as what they really are: a dynamic network. 

The lead’s start, end, and intersection points can be considered nodes, and the leads themselves as edges of a network. As the nodes and edges change over time, the ice lead network is constantly evolving. This new network perspective on ice leads could be of great interest for the cryospheric science community since it opens the door to new methods. For example, adapting common link prediction methods might make data-driven ice lead forecasting and tracking feasible.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/iceleads_distribution.png" title="Geographic distribution of Iceleads from our dataset." class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Geographic distribution of Iceleads from our dataset.
</div>


To reveal the hidden dynamics of ice leads, we performed a spatio-temporal and network analysis of ice lead networks. The networks used and presented here are based on daily ice lead observations from Moderate Resolution Imaging Spectroradiometer (MODIS) between 2002 and 2020 by Hoffman et al. [1](https://www.mdpi.com/2072-4292/11/5/521). 
The spatio-temporal analysis of the ice leads exhibits seasonal, annual, and overall trends in the ice lead dynamics. We found that the number of ice leads is decreasing, and the number of width and length outliers is increasing overall. The network analysis of the ice lead graphs reveals unique network characteristics that diverge from those present in common real-world networks.

Most notably, current network science methods (1) exploit the information that is embedded into the connections of the network, e.g., in connection clusters, while (2) nodes remain relatively fixed over time. Ice lead networks, however, (1) embed their relevant information spatially, e.g., in spatial clusters, and (2) shift and change drastically. These differences require improvements and modifications on common graph classification and link prediction methods such as Preferential Attachment and EvolveGCN on the domain of ice lead dynamic networks.
This work is a call for extending existing network analysis toolkits to include a new class of real-world dynamic networks. Utilizing network science techniques will hopefully further our understanding of ice leads and thus of Arctic processes that are key to climate change mitigation and adaptation.


<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div> -->


<!-- You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
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
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div> -->
```
{% endraw %}
