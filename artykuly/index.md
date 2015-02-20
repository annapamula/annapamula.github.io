---
title: artykuły
layout: post
---
{% for post in site.posts %}
<article class="preview">
    <p class="tagline">
        {{ post.date | date: "%-d %B %Y"}}
    </p>
    <h3>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </h3>
    <div class="excerpt" style="margin-top: 10px">
        <p>{{ post.excerpt }}</p>
    </div>
</article>
{% endfor %}
