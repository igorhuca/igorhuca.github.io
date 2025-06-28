---
layout: page
title: Todos os Posts
permalink: /pt/posts/
lang: pt
---

# Todos os Posts

{% assign posts = site.posts | where: "lang", "pt" %}

<div class="post-list">
  {% for post in posts %}
    <article class="post-preview">
      <h2><a href="{{ post.url | relative_url }}" class="post-link">{{ post.title }}</a></h2>
      <p class="post-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
        {% if post.categories.size > 0 %}
          • 
          {% for category in post.categories %}
            <span class="category">{{ category }}</span>
            {% unless forloop.last %}, {% endunless %}
          {% endfor %}
        {% endif %}
      </p>
      
      {% if post.excerpt %}
        <div class="post-excerpt">{{ post.excerpt }}</div>
      {% endif %}
      
      {% if post.tags.size > 0 %}
        <div class="post-tags-preview">
          {% for tag in post.tags %}
            <span class="tag-small">#{{ tag }}</span>
          {% endfor %}
        </div>
      {% endif %}
    </article>
  {% endfor %}
</div>

---

*Want to read in English? [View all posts in English]({{ '/posts/' | relative_url }})*