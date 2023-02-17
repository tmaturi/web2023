---
layout: default
title: Publications
---

# Publications

{% assign publications = site.data.publications %}

{% for publication in publications %}
## {{ publication.title }}

*Authors:* {{ publication.authors }}

*Year:* {{ publication.year }}

*Keywords:* {{ publication.keywords }}

[Link]({{ publication.link }})

{% endfor %}
