---
title: "GoodViBEs Lab - Pictures"
layout: piclay
excerpt: "GoodViBEs Lab -- Pictures"
permalink: /pictures/
---
---
title: "STMI Lab - Pictures"
layout: piclay
excerpt: "STMI Lab -- Pictures"
permalink: /pictures/
---

# Pictures

## Table of Contents

- [Pictures](#pictures)
  - [Conferences and Meetings](#conferences-and-meetings)
  - [Thesis Defense](#thesis-defense)
  - [ViBEs](#vibes)

## Conferences and Meetings

<div class="container">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
{% if pic.occasion == "Conferences and Meetings" %}
{% if number_printed | modulo: 3 == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if number_printed | modulo: 3 == 0 %}
</div>
{% endif %}
{% endif %}
{% endfor %}
{% if number_printed | modulo: 3 != 0 %}
</div>
{% endif %}
</div>

<p> &nbsp; </p>

## Thesis Defense

<div class="container">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
{% if pic.occasion == "Thesis Defense" %}
{% if number_printed | modulo: 3 == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if number_printed | modulo: 3 == 0 %}
</div>
{% endif %}
{% endif %}
{% endfor %}
{% if number_printed | modulo: 3 != 0 %}
</div>
{% endif %}
</div>

<p> &nbsp; </p>

## ViBEs

<div class="container">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
{% if pic.occasion == "ViBEs" %}
{% if number_printed | modulo: 3 == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if number_printed | modulo: 3 == 0 %}
</div>
{% endif %}
{% endif %}
{% endfor %}
{% if number_printed | modulo: 3 != 0 %}
</div>
{% endif %}
</div>

<p> &nbsp; </p>
