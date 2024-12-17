---
title: "GoodViBEs Lab - Pictures"
layout: piclay
excerpt: "GoodViBEs Lab -- Pictures"
permalink: /pictures/
---

# Pictures

## Table of Contents

- [Conferences and Meetings](#conferences-and-meetings)
- [Thesis Defense](#thesis-defense)
- [ViBEs](#vibes)

<style>
  .row {
    margin-bottom: 10px; /* Reduce space between rows */
  }
  .col-sm-4 {
    padding: 5px; /* Reduce padding around images */
  }
  img.img-responsive {
    margin: 0 auto; /* Center images */
    display: block;
  }
</style>

## Conferences and Meetings

<div class="row">
  {% assign number_printed = 0 %}
  {% for pic in site.data.pictures %}
    {% if pic.occasion == "Conferences and Meetings" %}
      <div class="col-sm-4">
        <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
          <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="100%" />
        </a>
      </div>
      {% assign number_printed = number_printed | plus: 1 %}
    {% endif %}
  {% endfor %}
</div>

<!-- Clear any float to avoid overlap -->
<div class="clearfix"></div>

## Thesis Defense

<div class="row">
  {% assign number_printed = 0 %}
  {% for pic in site.data.pictures %}
    {% if pic.occasion == "Thesis Defense" %}
      <div class="col-sm-4">
        <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
          <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="100%" />
        </a>
      </div>
      {% assign number_printed = number_printed | plus: 1 %}
    {% endif %}
  {% endfor %}
</div>

<!-- Clear any float to avoid overlap -->
<div class="clearfix"></div>

## ViBEs

<div class="row">
  {% assign number_printed = 0 %}
  {% for pic in site.data.pictures %}
    {% if pic.occasion == "ViBEs" %}
      <div class="col-sm-4">
        <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
          <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="100%" />
        </a>
      </div>
      {% assign number_printed = number_printed | plus: 1 %}
    {% endif %}
  {% endfor %}
</div>

<!-- Clear any float to avoid overlap -->
<div class="clearfix"></div>
