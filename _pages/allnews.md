---
title: "News"
layout: textlay
excerpt: "good ViBEs Lab at UPD."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<b>{{ article.keyword }}</b> <em>{{ article.headline }}</em></p>
{% endfor %}
