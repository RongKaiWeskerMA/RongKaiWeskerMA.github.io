---
layout: page
title:  Research
cover:  false
menu:   true
order:  1
---

<p align="center">
  <img src="/assets/img/herston.png" style="width: 400px; height: auto;">
  <em>A normal afternoon finishing work at Herston, the best office I've ever had!</em>
</p>


<ul>
{% for paper in site.data.papers.papers %}
  <li>
  {% include paper.html paper=paper %}
  </li>
{% endfor %}
</ul>

<audio autoplay="autoplay"> <source src="/assets/audio/Biesy.mp3" type="audio/mp3"> </audio>