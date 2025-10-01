---
layout: default
title: "Mijn Eerste Jekyll Pagina"
date: 2025-10-01
---

# Welkom bij mijn Jekyll-pagina

Vandaag leer je hoe Jekyll Markdown omzet naar HTML en Liquid gebruikt.

{% assign kerken = "Domkerk, St. Janskerk, Pieterskerk" | split: ", " %}

## Lijst van kerken in Utrecht
<ul>
{% for kerk in kerken %}
  <li>{{ kerk }}</li>
{% endfor %}
</ul>

**Vandaag is:** {{ "now" | date: "%A, %d %B %Y" }}
