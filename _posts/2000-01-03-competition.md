---
title: "competitions"
bg: orange
color: black
fa-icon: toggle-on
---

To be determined


{% for competition in site.competitions %}
  <h2>{{ competition.name }}</h2>
  <p>{{ competition.content  }}</p>
  <p>Languages/Skills: {{ competition.programming_language  }}</p>
  <p>Participant: {{ competition.participant }}</p>
  <p>Weight: {{ competition.weight }}</p>
{% endfor %}