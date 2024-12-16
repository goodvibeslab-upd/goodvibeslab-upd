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

{% assign number_printed = 0 %}
<div class="row">
{% for pic in site.data.pictures %}
  {% if pic.occasion == "Conferences and Meetings" %}
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="95%" />
      </a>
    </div>
    {% assign number_printed = number_printed | plus: 1 %}
    {% if number_printed == 3 %}
      </div>
      <div class="row">
      {% assign number_printed = 0 %}
    {% endif %}
  {% endif %}
{% endfor %}
</div>

<p> &nbsp; </p>

## Thesis Defense

{% assign number_printed = 0 %}
<div class="row">
{% for pic in site.data.pictures %}
  {% if pic.occasion == "Thesis Defense" %}
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="95%" />
      </a>
    </div>
    {% assign number_printed = number_printed | plus: 1 %}
    {% if number_printed == 3 %}
      </div>
      <div class="row">
      {% assign number_printed = 0 %}
    {% endif %}
  {% endif %}
{% endfor %}
</div>

<p> &nbsp; </p>

## ViBEs

{% assign number_printed = 0 %}
<div class="row">
{% for pic in site.data.pictures %}
  {% if pic.occasion == "ViBEs" %}
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="95%" />
      </a>
    </div>
    {% assign number_printed = number_printed | plus: 1 %}
    {% if number_printed == 3 %}
      </div>
      <div class="row">
      {% assign number_printed = 0 %}
    {% endif %}
  {% endif %}
{% endfor %}
</div>


<p> &nbsp; </p>
