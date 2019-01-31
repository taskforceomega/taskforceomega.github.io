---
layout: default
---

<div class="mos">
  {% for post in site.mos %}
    <article class="mos">

      <h1><a href="{{ site.baseurl }}{{ mos.url }}">{{ mos.title }}</a></h1>

      <div class="entry">
        {{ mos.excerpt }}
      </div>
      
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
      
      <div class="date">
        Posted on {{ mos.date | date: "%B %e, %Y" }}
      </div>
      
    </article>
  {% endfor %}
</div>
