---
layout: blog
permalink: /blog
title: Blog - Bearded Empire
description: The Bearded Empire blog is the ultimate guide to beard care, providing expert tips, product recommendations, and grooming routines to help you achieve a healthy, well-groomed beard that reflects your unique style and personality.
---

{% include header.html %}

<h1 class="text-center">Bearded Empire Blog</h1>

The ultimate guide to beard care, providing expert tips, product recommendations, and grooming routines to help you achieve a healthy, well-groomed beard that reflects your unique style and personality.

<hr>

## Latest Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>
        <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" fill="currentColor" class="bi bi-file-text" viewBox="0 0 16 16">
          <path d="M5 4a.5.5 0 0 0 0 1h6a.5.5 0 0 0 0-1H5zm-.5 2.5A.5.5 0 0 1 5 6h6a.5.5 0 0 1 0 1H5a.5.5 0 0 1-.5-.5zM5 8a.5.5 0 0 0 0 1h6a.5.5 0 0 0 0-1H5zm0 2a.5.5 0 0 0 0 1h3a.5.5 0 0 0 0-1H5z"/>
          <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V2zm10-1H4a1 1 0 0 0-1 1v12a1 1 0 0 0 1 1h8a1 1 0 0 0 1-1V2a1 1 0 0 0-1-1z"/>
      </svg>
      {{ post.post_excerpt }}
      </p>
      <p><small>Posted on: {{ post.date | date: "%m/%Y" }} &middot; Posted by: {{post.author}}</small></p>
    </li>
  {% endfor %}
</ul>

If you have content ideas or would like to contribute to our blog, please [contact us](mailto:beardedempireonline@gmail.com).

{% include footer.html %}
