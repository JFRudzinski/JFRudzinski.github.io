---
layout: "default-title"
title: "Teaching"
categories: jekyll Page
permalink: /_pages/teaching/
---

<!-- Pubs List -->
{% for post in site.categories.Class %}
<div class="image-container shadow center" >
  <div class="pub-preview">
    <article class="post-preview">
        <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        <h2 class="post-title">{{ post.title }}</h2>
        <h3 class="post-subtitle">{{post.semester}}</h3>
        <hr class="striped-border"> 
        </a>
    </article>
    <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
    <div class="after"></div>
    </a>
  </div>
</div>


<!-- <div class="container shadow center">
  <article class="post-preview">
  <div class="myDiv">
    <div class="subDiv">
      <img src="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }}" class="w-100" />
    </div>
  </div>
  </article>
</div> -->

<!-- <div
  class="bg-image hover-overlay ripple shadow-1-strong rounded"
  data-mdb-ripple-color="light"
>
  <img src="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }}" class="w-100" />
  <a href="#!">
    <div class="mask" style="background-color: rgba(251, 251, 251, 0.2)"></div>
  </a>
</div> -->


{% endfor %}


