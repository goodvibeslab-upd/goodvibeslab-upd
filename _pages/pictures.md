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



{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "Conferences and Meetings" %}
<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" data-lightbox="conferences-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/conferences-and-meetings/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

<p> &nbsp; </p>


{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "Thesis Defense" %}
<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" data-lightbox="thesis-defense-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/thesis-defense/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

<p> &nbsp; </p>


{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "ViBEs" %}
<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" data-lightbox="vibes-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/vibes/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

<p> &nbsp; </p>
