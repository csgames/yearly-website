---
title: "competitions"
bg: orange
color: black
fa-icon: toggle-on
---

<div class="container">
<div class="row">
{% for competition in site.competitions %}
<div class="five columns">
  <h4>{{ competition.name }}</h4>
    <p>{{ competition.content  }}</p>
    <p>Languages/Skills: {{ competition.programming_language }}</p>
    <p>Participant: {{ competition.participant }}</p>
    <p>Weight: {{ competition.weight }}</p>
</div>
  {% endfor %}
</div>
</div>