---
layout: "default-title"
title: "Publications"
categories: jekyll Page
---

<!-- Pubs List -->
{% for post in site.categories.Pub %}
<div class="image-container shadow center" >
  <div class="pub-preview">
    <article class="post-preview">
        <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        <h2 class="post-title">{{ post.title }}</h2>
        <h3 class="post-subtitle">{{post.authors}}, <i>{{post.journal}}</i> ({{ post.year }}) </h3>
        <hr class="striped-border"> 
        <picture height="900">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }} 2x"
                media="(max-width: 768px) and (-webkit-min-device-pixel-ratio: 1.5), (max-width: 768px) and (min-resolution: 144dpi)">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }} 2x"
                media="(max-width: 768px)">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }} 2x"
                media="(-webkit-min-device-pixel-ratio: 1.5), (min-resolution: 144dpi)">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }} 2x">
            <img src="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }}">
        </picture>
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


