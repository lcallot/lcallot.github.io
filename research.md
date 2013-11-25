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

{% for post in site.categories.papers limit:20 %} 
<article>
<h3><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h3>
<!---<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %Y" }}</time></span>-->
{% if post.coauthor %}Joint work with {{ post.coauthor }}.<br />{% endif %}
{% if post.status %}{{ post.status }}{% endif %}
</article>
{% endfor %}

