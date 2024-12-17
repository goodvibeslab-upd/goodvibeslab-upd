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
  /* Ensure proper spacing between sections */
  section {
    margin-bottom: 30px; /* Adds space between sections */
  }

  .row {
    margin-bottom: 20px; /* Space between image rows */
  }

  .col-sm-4 {
    padding: 5px; /* Padding for images */
  }

  img.img-responsive {
    margin: 0 auto; /* Center images */
    display: block;
    max-width: 100%; /* Ensure images scale properly */
  }

  /* Add margin to headers to ensure space above them */
  h2 {
    margin-top: 50px; /* Adds space above section headers */
    margin-bottom: 20px; /* Adds space below the headers */
  }
</style>

## Conferences and Meetings

<section id="conferences-and-meetings">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row clearfix">
{% endif %}
{% if pic.occasion == "Conferences and Meetings" %}
<div class="col-sm-4">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}
</section>

## Thesis Defense

<section id="thesis-defense">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row clearfix">
{% endif %}
{% if pic.occasion == "Thesis Defense" %}
<div class="col-sm-4">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}
</section>

## ViBEs

<section id="vibes">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row clearfix">
{% endif %}
{% if pic.occasion == "ViBEs" %}
<div class="col-sm-4">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}
</section>
