---
title: Image Index
layout: essay
order: 40
abstract: 'Featuring a grid of 631 figure images'
---

<div class="image-grid">

{% for figure in figures.figure_list %}
{% if figure.id contains "lamp" %}
  {% figure figure.id %}
{% endif %}
{% endfor %}

</div>
<style>
.image-grid {
  display: grid; 
  gap: 1rem;
  grid-template-columns: 1fr 1fr 1fr;
}
.image-grid .q-figure {
  border-width: 0;
  margin-bottom: 1rem !important;
  margin-top: 0 !important;
  padding: 0;
}
</style>