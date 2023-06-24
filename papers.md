---
layout: page
title:  Research
cover:  false
menu:   true
order:  1
---

> _Do not believe in anything simply because you have heard it.
> Do not believe in anything simply because it is spoken and rumored by many.
> Do not believe in anything simply because it is found written in your religious books. 
> Do not believe in anything merely on the authority of your teachers and elders.
> Do not believe in traditions because they have been handed down for many generations.
> But after observation and analysis, when you find that anything agrees with reason 
> and is conducive to the good and benefit of one and all, then accept it and live up to it._
>
> ---Guatama Shakyamunis

<ul>
{% for paper in site.data.papers.papers %}
  <li>
  {% include paper.html paper=paper %}
  </li>
{% endfor %}
</ul>

