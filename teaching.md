---
layout: page
permalink: /teaching/index.html
title: Teaching 
description: 
modified: 2013-11-19
tags: teaching
image:
  feature: monkey-lq.jpg
  credit: Laurent Callot 
---



{% for post in site.categories.teaching limit:20 %} 
<article>
<h3><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h3>
<!---<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %Y" }}</time></span>-->
</article>
{% endfor %}
