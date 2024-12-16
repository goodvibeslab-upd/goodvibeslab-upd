---
title: "GoodViBEs Lab - Pictures"
layout: piclay
excerpt: "GoodViBEs Lab -- Pictures"
permalink: /pictures/

---

# Pictures

## Conferences and Meetings

<div class="row">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
{% if pic.occasion == "Conferences and Meetings" %}
  <div class="col-sm-4 clearfix">
    <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
      <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="95%" />
    </a>
  </div>
  {% assign number_printed = number_printed | plus: 1 %}
  {% if number_printed == 3 %}
    </div> <!-- Close row after 3 images -->
    <div class="row"> <!-- Open new row -->
    {% assign number_printed = 0 %}
  {% endif %}
{% endif %}
{% endfor %}
</div> <!-- Close the last row -->

<p> &nbsp; </p>

## Thesis Defense

<div class="row">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
{% if pic.occasion == "Thesis Defense" %}
  <div class="col-sm-4 clearfix">
    <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
      <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="95%" />
    </a>
  </div>
  {% assign number_printed = number_printed | plus: 1 %}
  {% if number_printed == 3 %}
    </div> <!-- Close row after 3 images -->
    <div class="row"> <!-- Open new row -->
    {% assign number_printed = 0 %}
  {% endif %}
{% endif %}
{% endfor %}
</div> <!-- Close the last row -->

<p> &nbsp; </p>

## ViBEs

<div class="row">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
{% if pic.occasion == "ViBEs" %}
  <div class="col-sm-4 clearfix">
    <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
      <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="95%" />
    </a>
  </div>
  {% assign number_printed = number_printed | plus: 1 %}
  {% if number_printed == 3 %}
    </div> <!-- Close row after 3 images -->
    <div class="row"> <!-- Open new row -->
    {% assign number_printed = 0 %}
  {% endif %}
{% endif %}
{% endfor %}
</div> <!-- Close the last row -->
