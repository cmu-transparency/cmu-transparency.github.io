---
title: "Home"
layout: textlay
excerpt: "Accountable Systems Lab @ Carnegie Mellon University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
