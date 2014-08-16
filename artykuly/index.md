---
title: artykuły
layout: post
---
{% for post in site.posts limit: 5 %}
<article class="preview">
    <p class="tagline">
        {{ post.date | date: "%-d %B %Y"}}
    </p>
    <h3>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </h3>
    <div class="excerpt" style="margin-top: 10px">
        <p>Krótkie info o danym poście</p>
    </div>
</article>
{% endfor %}