---
layout: page
title: Development
permalink: /development/
---

<div class="home">

<ul class="post-list">
    {% for post in site.categories.development %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span> 
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <p>{{post.excerpt | remove: '<p>' | remove: '</p>'}}</p>
        
      </li>
    {% endfor %}
  </ul>

</div>