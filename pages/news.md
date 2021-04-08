---
layout: "default-title"
title: "News"
---

<!-- Pubs List -->
{% for post in site.categories.News %}
<div class="image-container shadow center" >
  <div class="pub-preview">
    <article class="post-preview">
        <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        <h2 class="post-title">{{ post.title }}</h2>
        <hr class="striped-border"> 
        <picture height="900">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/News/{{ post.year }}/{{ post.post-id }}/{{ post.titlepic }}.{{ post.titlepic_suff }} 2x"
                media="(max-width: 768px) and (-webkit-min-device-pixel-ratio: 1.5), (max-width: 768px) and (min-resolution: 144dpi)">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/News/{{ post.year }}/{{ post.post-id }}/{{ post.titlepic }}.{{ post.titlepic_suff }} 2x"
                media="(max-width: 768px)">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/News/{{ post.year }}/{{ post.post-id }}/{{ post.titlepic }}.{{ post.titlepic_suff }} 2x"
                media="(-webkit-min-device-pixel-ratio: 1.5), (min-resolution: 144dpi)">
            <source
                srcset="{{site.baseurl}}/assets/content/Images/News/{{ post.year }}/{{ post.id }}/{{ post.titlepic }}.{{ post.titlepic_suff }} 2x">
            <img src="{{site.baseurl}}/assets/content/Images/News/{{ post.year }}/{{ post.post-id }}/{{ post.titlepic }}.{{ post.titlepic_suff }}">
        </picture>
        <!-- <div class="post-excerpt"> <p>{% if post.excerpt %}{{post.excerpt | strip_html }}{% endif %}...</p> </div> -->
        </a>
    </article>
    <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
    <div class="after"></div>
    </a>
  </div>
</div>


{% endfor %}


