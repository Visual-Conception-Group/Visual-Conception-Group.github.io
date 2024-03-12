---
title: "VCG - Sponsored Projects"
layout: gridlay
excerpt: "VCG -- Sponsored Projects"
sitemap: false
permalink: /sponsored_projects/
---

## On-going Projects

{% for project in site.data.ongoing_projects %}

  <b>{{ project.title }}</b> <br />
  <em>{{ project.duration }} </em><br />{{ project.description }}
  {% if project.demolink != ""%}
  {{ project.demolink }}
  {% endif %}

{% endfor %}

## Completed Projects

{% for project in site.data.completed_projects %}

  <b>{{ project.title }}</b> <br />
  <em>{{ project.duration }} </em><br />{{ project.description }}

{% endfor %}