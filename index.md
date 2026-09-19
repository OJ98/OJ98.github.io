---
layout: default
title: Home
permalink: /
---

# Omkar Joshi

I am a PhD student in the Department of Computer Science at NC State University advised by <a href="https://www.csc2.ncsu.edu/faculty/mpsingh/">Dr. Munindar Singh</a>. My research focuses on multiagent systems, large language models and natural language processing.

## Research Interests

My work aims to understand how humans and agents reason and debate through language. I am particularly interested in:

- **Normative Multiagent Systems:** Building intelligent norm-aware agents that can operate in complex environments.
- **Computational Argumentation:** Extracting and evaluating argumentative structures in natural language.
- **Natural Language Understanding in the context of Debate Analysis:** Developing computational models to evaluate the quality and impact of rhetorical structures.

## Selected Publications

{% assign publications = site.research | where: "category", "publication"  | sort: "year" | reverse %}
{% for pub in publications limit: 3 %}
<div class="publication-item">
    <span class="publication-title"><a href="{{ pub.url | relative_url }}">{{ pub.title }}</a></span>
    <span class="publication-authors">{{ pub.authors }}</span><br>
    <span class="publication-venue">{{ pub.venue }} {{ pub.year }}, {{ pub.location }}</span>
</div>
{% endfor %}

[View all research →]({{ '/research/' | relative_url }})

---

<p class="sidenote">
I'm always interested in chatting about Multiagent Systems and Large Language Models. Feel free to reach out via email!
</p>
