---
title: "News"
layout: textlay
excerpt: "Materials Modelling Group"
sitemap: false
permalink: /allnews.html
---

&nbsp;

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
