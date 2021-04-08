---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default-home
keyvisual2: Cover_Image/Cover_Image
keyvisual2_suff: jpg
keyvisual1: Header/Header-edited # let's add the suffix as an additional variable
keyvisual1_suff: jpeg
---

{% for page in site.pages %}
  <h1>{{page.permalink}}</h1>
{% endfor %}

<!-- This is the carousel title -->
<div class="specials-grey">
<div class="center">
    <h1> Recent News </h1>
</div>
</div>

<head>
  <!-- other head stuff... -->
  <!-- <link rel="stylesheet" href="{{site.url}}/assets/css/flickity.css" media="screen"> -->
  <link rel="stylesheet" href="{{site.baseurl}}/assets/css/flickity.css" media="screen">
</head>

<!-- Start the carousel -->
<div class="container">
<body>
<!-- Flickity HTML init -->
<div class="carousel js-flickity">
  {% assign ctr = 0 %}
  {% for post in site.posts %} <!-- Loop over Pub and News posts -->
    {% if post.categories contains "Pub" %}
    {% assign ctr = ctr | plus:1 %}
    <div class="carousel-cell">
      <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        <div class="carousel-inner">
            <div class="active item">
            <div class="carousel-content">
                <h4>New publication on {{post.date | date: '%B %d, %Y'}}:</h4>
            </div>
            <div class="carousel-caption">
                <h5>{{post.title}}</h5>
            </div>
            <img src="{{site.baseurl}}/assets/content/Images/Pubs/{{ post.year }}/{{ post.pub-id }}/{{ post.pubtitlepic }}.{{ post.pubtitlepic_suff }}" alt="">
            </div>
        </div>
      </a>
    </div>
    {% elsif post.categories contains "News" %}
    {% assign ctr = ctr | plus:1 %}
    <div class="carousel-cell">
      <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
        <div class="carousel-inner">
            <div class="active item">
            <div class="carousel-content">
                <h4>New post on {{post.date | date: '%B %d, %Y'}}:</h4>
            </div>
            <div class="carousel-caption">
                <h5>{{post.title}}</h5>
            </div>
            <img src="{{site.baseurl}}/assets/content/Images/News/{{ post.year }}/{{ post.post-id }}/{{ post.titlepic }}.{{ post.titlepic_suff }}" alt="">
            </div>
        </div>
      </a>
    </div>
    {% endif %}  
    {% if ctr >= 5 %}
      {% break %}
    {% endif %}
  {% endfor %}
    <!-- Now add the last cell for linking to other pages -->
    <div class="carousel-cell">
        <div class="carousel-inner">
            <div class="active item">
            <div class="center">
                <a href="{{site.url}}/_pages/publications"><button class="carousel-button-2 shadow">More Publications</button></a>
            </div>
            <div class="center">
                <a href="{{site.url}}/_pages/news"><button class="carousel-button-1 shadow">More News</button></a>
            </div>
            <img src="{{site.url}}/assets/content/Images/Misc/blank.jpg" alt="">
            </div>
        </div>
    </div>
</div>
  <!-- all your great html... -->
  <script src="{{site.url}}/assets/css/flickity.pkgd.min.js"></script>
</body>
</div>

