---
layout: page
permalink: /papers/index.html
title: Research Papers 
description: "bla"
modified: 2013-11-19
tags: [research, ]
image:
  feature: kili-lq.jpg
  credit: Laurent Callot 
---

Paper titles are links to the abstract, pdf, and replication material. 

------------------------

## Peer-reviewed publications

{% for post in site.categories.pub limit:20 %} 
<article>
<h3><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h3>
<ul>
{% if post.coauthor %}<li>Joint work with {{ post.coauthor }}.</li>{% endif %}
{% if post.status %}<li>{{ post.status }}</li>{% endif %}
</ul>
</article>
{% endfor %}


------------------------

## Working papers

{% for post in site.categories.wp limit:20 %} 
<article>
<h3><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h3>
<ul>
{% if post.coauthor %}<li>Joint work with {{ post.coauthor }}.</li>{% endif %}
{% if post.status %}<li>{{ post.status }}</li>{% endif %}
</ul>
</article>
{% endfor %}
