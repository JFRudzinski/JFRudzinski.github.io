---
layout: "default-title"
title: "Software"
categories: jekyll Page
permalink: /_pages/software/
---

<!-- Pubs List -->
{% for post in site.categories.Pub %}
{% if post.data-label%}
{% if post.data-label contains "Software" %}
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
{% endif %}
{% endif %}
{% endfor %}


