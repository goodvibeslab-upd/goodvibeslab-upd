---
title: "GoodViBEs Lab - Pictures"
layout: piclay
excerpt: "GoodViBEs Lab -- Pictures"
permalink: /pictures/
---

# Pictures

{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 3 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
{% if pic.occasion == "mix" %}
<div class="col-sm-4 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/mix/{{ pic.image }}" data-lightbox="conferences-gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/mix/{{ pic.image }}" class="img-responsive" width="98%" style="float: left" />
  </a>
</div>
{% assign number_printed = number_printed | plus: 1 %}
{% endif %}
{% if even_odd == 2 %}
</div>
{% endif %}

{% endfor %}

<p> &nbsp; </p>
