---
layout: default
title: Research
permalink: /research/
---

# Research

My research explores the intersection of Natural Language Processing and computational social science, with a focus on argumentation and debate.

## Publications

{% assign publications = site.research | where: "category", "publication" | sort: "year" | reverse %}
{% for pub in publications %}
<div class="publication-item">
    <span class="publication-title"><a href="{{ pub.url | relative_url }}">{{ pub.title }}</a></span>
    <span class="publication-authors">{{ pub.authors }}</span><br>
    <span class="publication-venue">{{ pub.venue }}, {{ pub.year }}</span>
    {% if pub.description %}
    <p>{{ pub.description }}</p>
    {% endif %}
</div>
{% endfor %}

{% if publications.size == 0 %}
<p><em>No publications listed yet.</em></p>
{% endif %}

## Research in Progress

{% assign in_progress = site.research | where: "category", "in-progress" %}
{% for work in in_progress %}
<div class="publication-item">
    <span class="publication-title"><a href="{{ work.url | relative_url }}">{{ work.title }}</a></span>
    <p>{{ work.description }}</p>
</div>
{% endfor %}

{% if in_progress.size == 0 %}
<p><em>Check back soon for updates on current projects.</em></p>
{% endif %}
