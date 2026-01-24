---
layout: default
title: About
permalink: /about/
---

<div class="about-section">
    <div class="about-header">
        {% if site.author.avatar %}
        <img src="{{ site.author.avatar | relative_url }}" alt="{{ site.author.name }}" class="avatar">
        {% endif %}
        <div class="about-intro">
            <h1>{{ site.author.name }}</h1>
            <p><strong>{{ site.author.bio }}</strong></p>
            <p><em>{{ site.author.location }}</em></p>
        </div>
    </div>

    <h2>About Me</h2>
    <p>I'm a graduate student in the <a href="https://www.csc.ncsu.edu/" target="_blank">Computer Science Department</a> at <a href="https://www.ncsu.edu/" target="_blank">NC State</a>, pursuing a PhD in Computer Science advised by <a href="https://www.csc2.ncsu.edu/faculty/mpsingh/" target="_blank">Dr. Munindar Singh</a>.</p>

    <p>My research primarily focuses on the intersection of:</p>
    <ul>
        <li>Multiagent Protocols</li>
        <li>Natural Language Processing (NLP)</li>
        <li>Large Language Models (LLMs)</li>
        <li>Argumentation in NLP</li>
    </ul>

    <p>Currently, I'm working on a project that explores LLM-driven MultiAgent Protocols.</p>

    <h2>Outside of Research</h2>
    <p>In my free time, I enjoy playing board games and taking part in quizzes. I'm also an active participant in <a href="/files/Debate_Resume_Omkar.pdf" target="_blank">International British Parliamentary debates</a>, with several wins as both a debater and adjudicator. My passion for debate was instrumental in igniting my initial interest in Argumentation.</p>

    <p>I'm always excited to discuss and collaborate on projects or ideas. Feel free to reach out!</p>

    <h2>News</h2>
    <ul>
        <li><strong>[2025.8]</strong> Started my PhD in Computer Science at NC State!</li>
        <li><strong>[2023.8]</strong> Started my Masters in Computer Science at NC State!</li>
        <li><strong>[2023.7]</strong> Our paper, "ArgAnalysis35K" accepted and published to the main conference of ACL 2023!</li>
        <li><strong>[2022.9]</strong> Our paper, "A Proposal For An Interactive Parliamentary Debate Adjudication System" accepted and published in the Human-in-the-loop learning workshop at NeurIPS 2022</li>
    </ul>
</div>
