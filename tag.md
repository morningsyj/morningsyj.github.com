---
layout: page
title: Tags
permalink: /tag/
---
{% for tag in site.tags %}[{{ tag | first }}](#{{ tag | first }}) {% endfor %}

{% for tag in site.tags %}
<a name="{{ tag | first }}"><h2>#{{ tag | first }}</h2></a>

{% for post in tag.last %}
[{{ post.title }}]({{ post.url }}) <span class="pull-right">{{ post.date | date_to_string }}</span>
{% endfor %}{% endfor %}
