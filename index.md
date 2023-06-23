---
layout: page
title: About me
cover: true
---

I'm a Research Fellow at Data61, CSIRO ([ICV group](https://research.csiro.au/icv/)). I received my Ph.D. from Monash University (Australia), supervised by A/Prof. [Mehrtash Harandi](https://scholar.google.com/citations?user=Z9gvBegAAAAJ&hl=en) and Prof. [Tom Drummond](https://scholar.google.com/citations?user=6sWGL5wAAAAJ&hl=en). My recent research lies in efficient adaptation algorithms of deep learning models (Few-Shot Learning) for computer vision applications. 

Now, I'm currently interested and working on:
* 3D scene reconstruction and novel view synthesis (Neural Radiance Field).
* 3D reconstruction of surfaces/dense point cloud.

## Recent News
* I joined UCL as a Research Fellow under the supervision of Dr. [Pontus Stenetorp](https://pontus.stenetorp.se/) and Dr. [Pasquale Minervini](http://www.neuralnoise.com/)
* I did my internship at Amazon Search (Seattle, WA) (Jul-Oct, 2021)
* I did my internship at Adobe Research (San Jose, CA) (Jul-Sep, 2019)

## Recent Research Highlights

<ul>
{% for paper in site.data.papers.papers %}
  {% if paper.selected %}
  <li>
  {% include paper.html paper=paper %}
  </li>
  {% endif %}
{% endfor %}
</ul>

