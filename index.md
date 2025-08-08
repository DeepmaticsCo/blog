---
layout: default
title: Deepmatics
---

<div class="blog-cards-container">
    {% for post in site.posts %}
    <div class="blog-card">
        {% if post.image %}
            <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="card-image" />
        {% else %}
            <img src="{{ '/assets/prompt-engineering/header.png' | relative_url }}" alt="{{ post.title }}" class="card-image" />
        {% endif %}
        <div class="card-content">
            <h3 class="card-title">{{ post.title }}</h3>
            <p class="card-description">
                {% if post.excerpt %}
                    {{ post.excerpt | strip_html | truncatewords: 20 }}
                {% else %}
                    {{ post.content | strip_html | truncatewords: 20 }}
                {% endif %}
            </p>
            <a href="{{ post.url | relative_url }}" class="card-link">Read More</a>
        </div>
    </div>
    {% endfor %}
</div>