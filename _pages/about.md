---
permalink: /
layout: archive
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, this is Xiwen Wei (Christina), a second-year Electrical and Computer Engineering Ph.D. student at The University of Texas at Austin (UT Austin) since Fall 2023, advised by [Prof. Radu Marculescu](https://www.ece.utexas.edu/people/faculty/radu-marculescu). 
Before joining UT Austin, I received my B.S. degrees in Electrical Engineering at [University of Michigan, Ann Arbor](https://www.engin.umich.edu/), and in Electrical and Computer Engineering at [Shanghai Jiao Tong University](https://en.sjtu.edu.cn/). 

My research interests lie in continual learning and trustworthy AI. 

News
======

* [November 2024] [Online-LoRA](https://github.com/Christina200/Online-LoRA-official.git) got accepted by WACV. See you in Tucson!
* [October 2024] Two papers got accepted by 2nd Workshop on Regulatable ML and Continual FoMo Workshop @NeurIPS2024. See you in Vancuver!

Projects
======

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

