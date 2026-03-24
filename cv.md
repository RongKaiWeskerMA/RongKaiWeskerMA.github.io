---
layout: cinematic-page
title: CV
cover: false
menu: false
order: 6
---

{% for section in site.data.cv.before-pubs %}
<div class="cv-section">
  <div class="cv-section-title">{{ section.heading }}</div>
  {% if section.items %}
    {% for item in section.items %}
    <div class="cv-item">
      <div>
        <div class="cv-item-title">{{ item.title }}</div>
        <div class="cv-item-detail">{{ item.detail }}</div>
      </div>
      <div class="cv-item-year">{{ item.year }}</div>
    </div>
    {% endfor %}
  {% endif %}
  {% if section.subsections %}
    {% for sub in section.subsections %}
      {% for item in sub.items %}
      <div class="cv-item">
        <div>
          <div class="cv-item-title">{{ item.title }}</div>
          <div class="cv-item-detail">{{ item.detail }}</div>
        </div>
        <div class="cv-item-year">{{ item.year }}</div>
      </div>
      {% endfor %}
    {% endfor %}
  {% endif %}
</div>
{% endfor %}

<div class="cv-section">
  <div class="cv-section-title">Refereed Journal Articles</div>
  {% for paper in site.data.papers.papers %}
    {% if paper.venue == 'journal' %}
    <a class="paper-card" href="{{ paper.doc-url }}" target="_blank" rel="noopener">
      <div class="paper-meta">
        <span class="paper-venue">{{ paper.booktitle }}</span>
        <span class="paper-year">{{ paper.year }}</span>
      </div>
      <div class="paper-title">{{ paper.title }}</div>
      <div class="paper-authors">{{ paper.authors }}</div>
    </a>
    {% endif %}
  {% endfor %}
</div>

<div class="cv-section">
  <div class="cv-section-title">Refereed Conference Papers</div>
  {% for paper in site.data.papers.papers %}
    {% if paper.venue == 'conference' %}
    <a class="paper-card" href="{{ paper.doc-url }}" target="_blank" rel="noopener">
      <div class="paper-meta">
        <span class="paper-venue">{{ paper.booktitle | truncate: 60 }}</span>
        <span class="paper-year">{{ paper.year }}</span>
      </div>
      <div class="paper-title">{{ paper.title }}</div>
      <div class="paper-authors">{{ paper.authors }}</div>
    </a>
    {% endif %}
  {% endfor %}
</div>

{% for section in site.data.cv.after-pubs %}
<div class="cv-section">
  <div class="cv-section-title">{{ section.heading }}</div>
  {% if section.items %}
    {% for item in section.items %}
    <div class="cv-item">
      <div>
        <div class="cv-item-title">{{ item.title }}</div>
        <div class="cv-item-detail">{{ item.detail }}</div>
      </div>
      <div class="cv-item-year">{{ item.year }}</div>
    </div>
    {% endfor %}
  {% endif %}
  {% if section.subsections %}
    {% for sub in section.subsections %}
      {% for item in sub.items %}
      <div class="cv-item">
        <div>
          <div class="cv-item-title">{{ item.title }}</div>
          <div class="cv-item-detail">{{ item.detail }}</div>
        </div>
        <div class="cv-item-year">{{ item.year }}</div>
      </div>
      {% endfor %}
    {% endfor %}
  {% endif %}
</div>
{% endfor %}
