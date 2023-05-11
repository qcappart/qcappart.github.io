---
title: Publications
permalink: /publications/
author_profile: true
---

A list of my publications is available on my [google scholar profile](https://scholar.google.com/citations?user=QJQMYLsAAAAJ&hl). \
You can also see some project highlights on my [research group webpage](https://corail-research.github.io/publications/).

{% for publi in site.data.publist %}
  * {{ publi.title }} <br />
   <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endfor %}
