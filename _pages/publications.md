---
title: "VCG - Research"
layout: gridlay
excerpt: "VCG -- Research"
sitemap: false
permalink: /publications/
---


# Publications


(For a full list of publications see [below](#journal-publications) and for conference presentations, go [here](#conferences--workshops) or go to [Google Scholar](https://scholar.google.co.in/citations?user=aPDRgKAAAAAJ&hl=en))

<!-- ## Group highlights
{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p> -->

## Journal Publications

{% for publi in site.data.journal_publist %}

  <b> {{ publi.title }} </b> <br />
  <em>{{ publi.authors }} </em><br />
  {{ publi.journal }} <br />
  {% if publi.link.local == 1 %}
  <a href="{{ site.url }}{{ site.baseurl }}/downloads/{{ publi.link.url }}">{{ publi.link.display }}</a> <br />
  {% endif %}
  {% if publi.link.local == 0 %}
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a> <br />
  {% endif %}
  <!-- IF: {{ publi.IF }} -->

{% endfor %}

## Conferences & Workshops

{% for publi in site.data.conf_publist %}

  <b> {{ publi.title }} </b> <br />
  <em>{{ publi.authors }} </em><br />
  {{ publi.venue }} <br />
  {% if publi.link.local == 1 %}
  <a href="{{ site.url }}{{ site.baseurl }}/downloads/{{ publi.link.url }}">{{ publi.link.display }}</a> <br />
  {% endif %}
  {% if publi.link.local == 0 %}
  <a href="{{ publi.link.url }}">{{ publi.link.display }}</a> <br />
  {% endif %}

{% endfor %}
