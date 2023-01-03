---
layout: default
title: Blog
nav_order: 3
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /blog
---

 <div class="posts">
    {% for post in site.posts limit:10 %}
   
  
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
  
     
        <!-- <img src="{{post.image}}"><br> -->
  
        {{ post.excerpt }}
      
  
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>

      <hr/>
   
    {% endfor %}
  </div>
