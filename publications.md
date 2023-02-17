---
layout: default
title: Publications
---

# Publications

<div class="search-box">
  <form>
    <label for="year">Year:</label>
    <input type="text" id="year" name="year">
    <label for="keywords">Keywords:</label>
    <input type="text" id="keywords" name="keywords">
    <button type="submit">Search</button>
  </form>
</div>



{% assign publications = site.data.publications %}

{% for publication in publications %}
## {{ publication.title }}

*Authors:* {{ publication.authors }}

*Year:* {{ publication.year }}

*Keywords:* {{ publication.keywords }}

[Link]({{ publication.link }})

{% endfor %}
