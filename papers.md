---
layout: page
title:  Research
cover:  false
menu:   true
order:  1
---

<img title="Herston" alt="Alt text" src="/assets/img/herston.png" style="display: block; margin-left: auto; margin-right: auto; width: 400px;" />

<ul>
{% for paper in site.data.papers.papers %}
  <li>
  {% include paper.html paper=paper %}
  </li>
{% endfor %}
</ul>

<audio autoplay="autoplay"> <source src="/assets/audio/Biesy.mp3" type="audio/mp3"> </audio>