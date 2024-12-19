---
title: Publications
permalink: /publications/
author_profile: true
---

A list of my publications is available on my [google scholar profile](https://scholar.google.com/citations?user=QJQMYLsAAAAJ&hl). \
You can also see some project highlights on my [research group webpage](https://corail-research.github.io/publications/).

## 2025

{% for publi in site.data.publist %}
  {% if publi.year == 2025 %}
  * {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% endif %}
{% endfor %}

## 2024

{% for publi in site.data.publist %}
  {% if publi.year == 2024 %}
  * {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% endif %}
{% endfor %}


## 2023

{% for publi in site.data.publist %}
  {% if publi.year == 2023 %}
  * {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% endif %}
{% endfor %}

## 2022

{% for publi in site.data.publist %}
  {% if publi.year == 2022 %}
  * {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% endif %}
{% endfor %}

## 2021

{% for publi in site.data.publist %}
  {% if publi.year == 2021 %}
  * {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% endif %}
{% endfor %}

## 2020 and before

{% for publi in site.data.publist %}
  {% if publi.year <= 2020 %}
  * {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% endif %}
{% endfor %}