---
layout: default
title: "Business Technology Articles"
description: "Peter Karousis writes about cybersecurity, software choices, and everyday AI tools for small businesses in the Mahoning Valley."
permalink: /blog/
---
<p><a href="/">Diamond Tech Solutions home</a></p>
<h1>Diamond Tech Blog</h1>
<ul>
  {% for post in site.posts %}
    {% unless post.hide_from_index %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a> · <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></li>
    {% endunless %}
  {% endfor %}
</ul>
