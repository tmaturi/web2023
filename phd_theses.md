---
layout: default
title: PhD Theses
---

# PhD Theses

{% assign theses = site.data.phd_theses %}

{% for thesis in theses %}
## {{ thesis.title }}

*Author:* {{ thesis.author }}

*Year:* {{ thesis.year }}

*Keywords:* {{ thesis.keywords }}

[Link]({{ thesis.link }})

{% endfor %}
