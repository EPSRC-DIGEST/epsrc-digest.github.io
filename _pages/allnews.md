---
title: "News"
layout: textlay
excerpt: "DIGEST project at Oxford University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p><b>{{ article.date }}</b><br>
<em>{{ article.headline }}</em></p>
{% endfor %}
