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
   <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="10%" style="float: left; margin-right: 15px;" />
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

<div class="well-sm">
<ul class="flex-container">
<li class="flex-item1">
  {% if publi.image %}
   <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="200%" style="float: left" />
  {% endif %}
</li>
<li class="flex-item2">
  <strong> {{ publi.title }}</strong> <br />
  <em>{{ publi.authors }} </em><br />
  {{ publi.display }} {% if publi.year %}({{publi.year}}){% endif %}<br/>
  {% if publi.link.url %}<a href="{{ site.url }}{{ site.baseurl }}/papers/{{ publi.link.url }}.pdf" target="_blank"><button class="btn-pdf">PDF</button></a>{% endif %}
  {% if publi.doi %}<a href="http://dx.doi.org/{{ publi.doi }}" target="_blank"><button class="btn-doi">DOI</button></a> {% endif %}
  {% if publi.arxiv %}<a href="https://arxiv.org/abs/{{ publi.arxiv }}" target="_blank"><button class="btn-arxiv">ARXIV</button></a> {% endif %}
  {% if bibtest == true %} <a data-toggle="collapse" href="#{{ publi.link.url }}2" class="btn-bib" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{ publi.link.url }}2">BIB</a> {% endif %}
  {% if publi.abstract %} <a data-toggle="collapse" href="#{{ publi.link.url }}" class="btn-abstract" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{ publi.link.url }}">ABSTRACT</a>{% endif %}

{% if publi.abstract %}
<br/>
<div class="collapse" id="{{ publi.link.url }}"><div class="well-abstract">
 {{publi.abstract}}
</div></div>
{% endif %}

</li>
</ul>

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
