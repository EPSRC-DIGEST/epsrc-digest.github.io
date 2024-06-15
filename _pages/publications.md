---
title: "DIGEST project - Publications"
layout: gridlay
excerpt: "DIGEST project -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

## Group highlights

**At the end of this page, you can find the [full list of publications and patents](#full-list-of-publications). All papers are also available on [arXiv](https://arxiv.org/search/?query=Howey+David&searchtype=author&abstracts=show&order=-announced_date_first&size=50).**

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% if publi.highlight == 1 %}

<div class="clearfix">
 <div class="well">
   <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="15%" style="float: left; margin-right: 15px;" />
  <pubtit>{{ publi.title }}</pubtit>
  <p>{{ publi.authors }}</p>
  {% if publi.link.url %}<a href="{{ publi.link.url }}" target="_blank"><button class="btn-pdf">PDF</button></a>{% endif %}
  <button class="btn-abstract" onclick="toggleAbstract('abstract{{ forloop.index }}')">ABSTRACT</button>
  <div id="abstract{{ forloop.index }}" class="abstract-content" style="display:none;">
    <p>{{ publi.description }}</p>
  </div>
  <p class="text-danger"><strong>{{ publi.news1 }}</strong></p>
  <p>{{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endif %}
{% endfor %}

<p> &nbsp; </p>

## Full List of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }}</em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
