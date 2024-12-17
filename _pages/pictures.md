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
  h2 {
    margin-top: 30px; /* Add space above section headers */
    margin-bottom: 20px; /* Add space below section headers */
    font-size: 1.5em; /* Adjust font size for headers */
  }
  .row {
    margin-bottom: 15px; /* Space between image rows */
  }
  .col-sm-4 {
    padding: 5px; /* Space around images */
  }
  img {
    margin: 0 auto; /* Center images */
    display: block;
    width: 95%; /* Uniform image width */
  }
</style>

## Conferences and Meetings

<h2 id="conferences-and-meetings">Conferences and Meetings</h2>

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "Conferences and Meetings" %}
<div class="col-sm-4">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" alt="Conference Image" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

## Thesis Defense

<h2 id="thesis-defense">Thesis Defense</h2>

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "Thesis Defense" %}
<div class="col-sm-4">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" alt="Thesis Defense Image" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

## ViBEs

<h2 id="vibes">ViBEs</h2>

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "ViBEs" %}
<div class="col-sm-4">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" alt="ViBEs Image" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}
