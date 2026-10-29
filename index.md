---
layout: default
title: Home
permalink: /
---

# Omkar Joshi

I am a PhD student in the Department of Computer Science at NC State University advised by <a href="https://www.csc2.ncsu.edu/faculty/mpsingh/">Dr. Munindar Singh</a>. My research focuses on multiagent systems, large language models and natural language processing.

## Research Interests

My research focuses on building intelligent systems that reason, communicate, and make decisions through natural language. I am particularly interested in:
- <b>LLM-Based Agents and Multiagent Systems:</b> Designing autonomous agents that coordinate through interaction protocols, reason about norms, and operate reliably in complex environments.
- <b>Reliable AI and Decision Support:</b> Investigating how reasoning, structured knowledge, feedback, and evaluation mechanisms can improve the reliability of LLM-based systems in complex decision-making tasks.
- <b>Computational Argumentation:</b> Developing computational methods to extract, analyze, and evaluate arguments, rhetorical strategies, and the quality of natural-language reasoning.

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
