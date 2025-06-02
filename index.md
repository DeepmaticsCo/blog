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
    
    {% if site.posts.size == 0 %}
    <!-- Fallback if no posts are found -->
    <div class="blog-card">
        <img src="{{ '/assets/gemma3/Gemma3_KeywordBlog_RD3.png' | relative_url }}" alt="Gemma3" class="card-image" />
        <div class="card-content">
            <h3 class="card-title">Google Gemma3 Release</h3>
            <p class="card-description">Gemma 3 comes in a range of sizes (1B, 4B, 12B and 27B).</p>
            <a href="{{ '/ai-ml/gemma-3-release.html' | relative_url }}" class="card-link">Read More</a>
        </div>
    </div>
    <div class="blog-card">
        <img src="{{ '/assets/prompt-engineering/header.png' | relative_url }}" alt="Prompt Engineering Guide" class="card-image" />
        <div class="card-content">
            <h3 class="card-title">Prompt Engineering Guide</h3>
            <p class="card-description">This series (WIP) is a guide to effective prompting!</p>
            <a href="{{ '/ai-ml/prompting-series.html' | relative_url }}" class="card-link">Read More</a>
        </div>
    </div>
    {% endif %}
</div>