---
layout: default
title: Projects
permalink: /projects/
---

<h1>Projects</h1>

<p>Here are some of the projects I've been working on. Click on any project to learn more.</p>

<div class="projects-grid">
    {% for project in site.projects %}
    <div class="project-card">
        {% if project.image %}
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
        {% endif %}
        <div class="project-content">
            <h3>{{ project.title }}</h3>
            <p>{{ project.description }}</p>
            <a href="{{ project.url | relative_url }}" class="project-link">Learn More →</a>
        </div>
    </div>
    {% endfor %}
</div>

{% if site.projects.size == 0 %}
<p><em>Projects coming soon. Check back later!</em></p>
{% endif %}
