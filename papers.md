---
layout: cinematic-page
title: Research
subtitle: "The only way to deal with an unfree world is to become so absolutely free that your very existence is an act of rebellion. — Albert Camus"
cover: false
menu: true
order: 1
cover_image: /assets/img/sunshine.png
---

<div style="text-align:center; margin-bottom:2rem;">
<img re-ignore src="/assets/img/sunshine.png" style="max-width:100%; border-radius:8px;" />
</div>

<div>
{% for paper in site.data.papers.papers %}
<a class="paper-card" href="{{ paper.doc-url }}" target="_blank" rel="noopener">
<div class="paper-meta">
<span class="paper-venue">{{ paper.booktitle | truncate: 60 }}</span>
<span class="paper-year">{{ paper.year }}</span>
</div>
<div class="paper-title">{{ paper.title }}</div>
<div class="paper-authors">{{ paper.authors }}</div>
</a>
{% endfor %}
</div>

<audio autoplay loop> <source src="/assets/audio/unter.mp3" type="audio/mp3"> </audio>
