---
layout: default
title: Contact
permalink: /contact/
---

<h1>Get In Touch</h1>

<p>I'm always interested in hearing about exciting projects and new ideas. Feel free to reach out!</p>

<div class="contact-form">
    <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
        <div class="form-group">
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>
        </div>

        <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
        </div>

        <div class="form-group">
            <label for="message">Message</label>
            <textarea id="message" name="message" required></textarea>
        </div>

        <button type="submit" class="btn btn-primary">Send Message</button>
    </form>
</div>

<hr style="margin: 3rem 0;">

<h2>Other Ways to Connect</h2>

<ul style="list-style: none; padding: 0;">
    {% if site.author.email %}
    <li style="margin-bottom: 1rem;">
        <strong>Email:</strong> <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a>
    </li>
    {% endif %}
    
    {% if site.author.github %}
    <li style="margin-bottom: 1rem;">
        <strong>GitHub:</strong> <a href="https://github.com/{{ site.author.github }}" target="_blank">{{ site.author.github }}</a>
    </li>
    {% endif %}
    
    {% if site.author.googlescholar %}
    <li style="margin-bottom: 1rem;">
        <strong>Google Scholar:</strong> <a href="{{ site.author.googlescholar }}" target="_blank">My Profile</a>
    </li>
    {% endif %}
</ul>

<hr style="margin: 3rem 0;">

<p><em>Note: The contact form above requires setup. Visit <a href="https://formspree.io" target="_blank">Formspree</a> to create a free form endpoint and replace YOUR_FORM_ID.</em></p>
