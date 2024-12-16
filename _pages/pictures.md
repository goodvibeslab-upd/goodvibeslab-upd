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

## Conferences and Meetings

<div class="row">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
  {% if pic.occasion == "Conferences and Meetings" %}
    {% assign even_odd = number_printed | modulo: 3 %}
    {% if even_odd == 0 and number_printed != 0 %}
      </div> <!-- Close the previous row -->
      <div class="row"> <!-- Start a new row -->
    {% endif %}
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="95%" />
      </a>
    </div>
    {% assign number_printed = number_printed | plus: 1 %}
  {% endif %}
{% endfor %}
</div>

<p> &nbsp; </p>

## Thesis Defense

<div class="row">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
  {% if pic.occasion == "Thesis Defense" %}
    {% assign even_odd = number_printed | modulo: 3 %}
    {% if even_odd == 0 and number_printed != 0 %}
      </div> <!-- Close the previous row -->
      <div class="row"> <!-- Start a new row -->
    {% endif %}
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="95%" />
      </a>
    </div>
    {% assign number_printed = number_printed | plus: 1 %}
  {% endif %}
{% endfor %}
</div>

<p> &nbsp; </p>

## ViBEs

<div class="row">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
  {% if pic.occasion == "ViBEs" %}
    {% assign even_odd = number_printed | modulo: 3 %}
    {% if even_odd == 0 and number_printed != 0 %}
      </div> <!-- Close the previous row -->
      <div class="row"> <!-- Start a new row -->
    {% endif %}
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="95%" />
      </a>
    </div>
    {% assign number_printed = number_printed | plus: 1 %}
  {% endif %}
{% endfor %}
</div>

