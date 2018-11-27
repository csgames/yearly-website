---
title: "competitions"
bg: orange
color: white
fa-icon: toggle-on
---


{% for competition in site.competitions %}
{% assign mod = forloop.index | modulo: 2 %}

{% if mod == 1 %}
<div class="row">
{% endif %}
  <div class="one-half column">
    <h4>{{ competition.name }}</h4>
      <p>{{ competition.content  }}</p>
      <p>Languages/Skills: {{ competition.programming_language }}</p>
      <p>Participant: {{ competition.participant }}</p>
      <p>Weight: {{ competition.weight }}</p>
  </div>
{% if mod == 0 %}
</div>
{% endif %}
{% endfor %}

