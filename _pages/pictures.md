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
{% for pic in site.data.pictures %}
  {% if pic.occasion == "Conferences and Meetings" %}
    {% assign even_odd = number_printed | modulo: 3 %}
    
    {% if even_odd == 0 %}
      <div class="row">
    {% endif %}
    
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-and-meetings-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
      </a>
    </div>
    
    {% assign number_printed = number_printed | plus: 1 %}
    
    {% if even_odd == 2 %}
      </div> <!-- Close the row after 3 images -->
    {% endif %}
  {% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd != 0 %}
  </div> <!-- Close the last row if it wasn't closed -->
{% endif %}

<p> &nbsp; </p>

## Thesis Defense

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
  {% if pic.occasion == "Thesis Defense" %}
    {% assign even_odd = number_printed | modulo: 3 %}
    
    {% if even_odd == 0 %}
      <div class="row">
    {% endif %}
    
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
      </a>
    </div>
    
    {% assign number_printed = number_printed | plus: 1 %}
    
    {% if even_odd == 2 %}
      </div> <!-- Close the row after 3 images -->
    {% endif %}
  {% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd != 0 %}
  </div> <!-- Close the last row if it wasn't closed -->
{% endif %}

<p> &nbsp; </p>

## ViBEs

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}
  {% if pic.occasion == "ViBEs" %}
    {% assign even_odd = number_printed | modulo: 3 %}
    
    {% if even_odd == 0 %}
      <div class="row">
    {% endif %}
    
    <div class="col-sm-4 clearfix">
      <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
        <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
      </a>
    </div>
    
    {% assign number_printed = number_printed | plus: 1 %}
    
    {% if even_odd == 2 %}
      </div> <!-- Close the row after 3 images -->
    {% endif %}
  {% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 3 %}
{% if even_odd != 0 %}
  </div> <!-- Close the last row if it wasn't closed -->
{% endif %}
