---
title: "News"
layout: textlay
excerpt: "DIGEST project at Oxford University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
{{ article.date }} <br> {{ article.headline | markdownify}}
{% endfor %}
