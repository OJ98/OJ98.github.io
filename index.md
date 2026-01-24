---
layout: default
title: Home
permalink: /
---

<section class="hero">
    <h1>Hi, I'm {{ site.author.name }}</h1>
    <p>{{ site.author.bio }} in {{ site.author.location }}</p>
    
    <div class="cta-buttons">
        <a href="{{ '/projects/' | relative_url }}" class="btn btn-primary">View My Projects</a>
        <a href="{{ '/about/' | relative_url }}" class="btn btn-secondary">Learn More</a>
    </div>
</section>

<section>
    <h2>Featured Projects</h2>
    
    <div class="projects-grid">
        {% for project in site.projects limit:3 %}
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

    <div style="text-align: center; margin-top: 2rem;">
        <a href="{{ '/projects/' | relative_url }}" class="btn btn-primary">See All Projects</a>
    </div>
</section>
