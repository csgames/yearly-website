---
title: "competitions"
bg: orange
color: black
fa-icon: toggle-on
---

To be determined
<div class="row">
{% for competition in site.competitions %}
<div class="column">
  <h3>{{ competition.name }}</h3>
    <p>{{ competition.content  }}</p>
    <p>Languages/Skills: {{ competition.programming_language  }}</p>
    <p>Participant: {{ competition.participant }}</p>
    <p>Weight: {{ competition.weight }}</p>
</div>
  {% endfor %}
</div>