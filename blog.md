---
layout: page
title: Blog: Blog_name
permalink: /blog/
---

My posts generally fall under one of three categories: 

* COMMENT: Discussion of either work that I have found interesting or recent pop-science claims (in the fields of Cognitive Science and Linguistics).

* SUMMARY: Discussion of my own recent work.

* MUSING: Anything else.

&nbsp;

Read my posts below:

---

&nbsp;

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
      
      <div class="date">
        {{ post.date | date: "%B %e, %Y" }}
      </div>
      
      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
