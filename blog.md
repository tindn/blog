---
layout: default
---

<div class="home">

  <!--<h1 class="page-heading">Posts</h1>-->

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <span class="post-meta">posted on {{ post.date | date: "%b %-d, %Y" }} in <a href="/{{post.categories}}" target="_blank">{{post.categories}}</a></span> 
        <p>{{post.excerpt | remove: '<p>' | remove: '</p>'}}</p>
        
      </li>
    {% endfor %}
  </ul>
  <!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->

</div>
