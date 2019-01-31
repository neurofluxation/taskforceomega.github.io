---
layout: default
---

<div class="mos">
  {% for post in site.mos %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>
      
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
      
      <div class="date">
        Posted on {{ post.date | date: "%B %e, %Y" }}
      </div>
      
    </article>
  {% endfor %}
</div>