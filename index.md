---
layout: default
title: Home
permalink: /
---

# Omkar Joshi

I am a {{ site.author.bio }} at NC State University. My research focuses on computational linguistics, argumentation mining, and natural language processing.

## Research Interests

My work aims to understand how humans reason and debate through language. I am particularly interested in:

- **Argumentation Mining:** Extracting and analyzing argumentative structures in text.
- **Debate Analysis:** Developing computational models to evaluate the quality and impact of debate.
- **Natural Language Understanding:** Improving how models represent complex rhetorical structures.

## Selected Publications

{% assign publications = site.research | where: "category", "publication" %}
{% for pub in publications limit: 3 %}
<div class="publication-item">
    <span class="publication-title"><a href="{{ pub.url | relative_url }}">{{ pub.title }}</a></span>
    <span class="publication-authors">{{ pub.authors }}</span><br>
    <span class="publication-venue">{{ pub.venue }}, {{ pub.year }}</span>
</div>
{% endfor %}

[View all research →]({{ '/research/' | relative_url }})

---

<p class="sidenote">
I am currently seeking collaborations on projects involving argumentation and Large Language Models. Feel free to reach out via email.
</p>
