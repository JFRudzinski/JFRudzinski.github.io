---
layout: "default-title"
title: "Group Members"
PI-name: Joseph F. Rudzinski
PI-title: Group Leader
PI-pic: Members/JFR # assumes in content/Images/
PI-pic_suff: jpeg
---

<!---PI section--->
<section id="member-PI">
    <div class="container">
        <div class="col-xs-12 col-sm-12 col-md-6">
            <!-- <h5 class="center">{{ page.PI-title }}</h5> -->
            <p><span>Joseph received a Bachelors in chemistry and mathematics from the University of California, Santa Barbara in 2009. In 2014, he completed his Ph.D. in theoretical chemistry at The Pennsylvania State University in the group of Professor Will Noid, studying statistical-mechanics-based methods for constructing coarse-grained simulation models. Joseph moved to Mainz in 2015 to work on the interpretation of coarse-grained dynamics at the Max Planck Institute for Polymer Research, under the supervision of Kurt Kremer and Tristan Bereau. He received a Humboldt Postdoctoral Fellowship in 2016 to develop methods for constructing kinetically-consistent coarse-grained models for peptides. Joseph has been working as a group leader since January 2020, with a focus on developing multiscale simulation methodologies and investigating the interactions and conformational dynamics of disordered biological polymers.</span></p>  
        </div>
        <div class="col-xs-12 col-sm-6 col-md-3 col-md-offset-1">
            <ul class="keyvisual" height="900">
                <picture height="900">
                    <h2>{{ page.PI-title }}</h2>
                    <source
                        srcset="{{site.baseurl}}/assets/content/Images/{{ page.PI-pic }}.{{ page.PI-pic_suff }} 2x"
                        media="(max-width: 768px) and (-webkit-min-device-pixel-ratio: 1.5), (max-width: 768px) and (min-resolution: 144dpi)">
                    <source
                        srcset="{{site.baseurl}}/assets/content/Images/{{ page.PI-pic }}.{{ page.PI-pic_suff }} 2x"
                        media="(max-width: 768px)">
                    <source
                        srcset="{{site.baseurl}}/assets/content/Images/{{ page.PI-pic }}.{{ page.PI-pic_suff }} 2x"
                        media="(-webkit-min-device-pixel-ratio: 1.5), (min-resolution: 144dpi)">
                    <source
                        srcset="{{site.baseurl}}/assets/content/Images/{{ page.PI-pic }}.{{ page.PI-pic_suff }} 2x">
                    <img src="{{site.baseurl}}/assets/content/Images/{{ page.PI-pic }}.{{ page.PI-pic_suff }}">
                </picture>
                <div class="carousel-caption"> <h4><span class="caption-style"> {{ page.PI-name }} </span> </h4> </div>
            </ul>
        </div>
    </div>
    <div class="container">
        <h3>Publication Summary as of April 07, 2021: </h3><h3 class=center> <a href="https://scholar.google.com/citations?user=8DuZOHUAAAAJ&hl=en" target="_blank"><button class="button-new shadow">Google Scholar</button></a> </h3>
        <div class="col-xs-12 col-sm-12 col-md-6">
          <img src="{{site.baseurl}}/assets/content/Images/Members/Citations.jpg">
        </div>
        <div class="col-xs-12 col-sm-6 col-md-6">
          <img src="{{site.baseurl}}/assets/content/Images/Members/Pub_Dist.jpg"> 
        </div>
    </div>
  </section>

  <hr class="striped-border">

<!-- Member List -->
{% for post in site.categories.Memb %}

<section id="member">
      <div class="container">
        <div class="col-xs-12 col-sm-6 col-md-3 col-md-offset-1">
            <ul class="keyvisual">
                <picture>
                    <h2>{{ post.title }}</h2>
                    <img src="{{site.baseurl}}/assets/content/Images/{{ post.pic }}.{{ post.pic_suff }}">
                </picture>
                <div class="carousel-caption"> <h4><span class="caption-style"> {{ post.name }} </span> </h4> </div>
            </ul>
        </div>
        <div class="col-xs-12 col-sm-12 col-md-6 col-md-offset-1"> 
            <ul class="keyvisual-memb">
                <picture>
                    <img src="{{site.baseurl}}/assets/content/Images/{{ post.res-pic }}.{{ post.res-pic_suff }}">
                    <h2 class="center">{{ post.project }}</h2>
                </picture>
            </ul>
        </div>
    </div>
  </section>


  {% endfor %}