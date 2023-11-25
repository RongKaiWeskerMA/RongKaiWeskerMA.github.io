---
layout: page
title: About me
cover: true
---

I'm a Research Fellow at Data61, CSIRO ([ICV group](https://research.csiro.au/icv/)). I received my Ph.D. from Monash University (Australia), supervised by A/Prof. [Mehrtash Harandi](https://scholar.google.com/citations?user=Z9gvBegAAAAJ&hl=en) and Prof. [Tom Drummond](https://scholar.google.com/citations?user=6sWGL5wAAAAJ&hl=en). I completed my bachelor degree at Monash University and Central University (2+2 program). My previous research interest largely lies in efficient adaptation algorithms for deep learning models (Few-Shot Learning) in the context of computer vision.   

Now, I'm currently interested and have been working on:
* 3D scene reconstruction and novel view synthesis (Neural Radiance Field).
* 3D reconstruction of surfaces/dense point cloud from imges.

## Recent News
* I will join Nvidia as a senior machine learning engineer next year! (Shanghai)
* I joined CSIRO as a Research Fellow since Feb, 2023 (Brisbane).
* I completed the Ph.D degree in Dec, 2022 (Melbourne).

<audio autoplay="autoplay"> <source src="/assets/audio/sleeping_lotus.mp3" type="audio/mp3"> </audio>

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

