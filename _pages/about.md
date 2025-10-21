---
permalink: /
layout: archive
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, this is Xiwen Wei (Christina), a second-year Electrical and Computer Engineering Ph.D. student at [The University of Texas at Austin (UT Austin)](https://www.ece.utexas.edu/) since Fall 2023. 
Before joining UT Austin, I received my B.S. degrees in Electrical Engineering at [University of Michigan, Ann Arbor](https://www.engin.umich.edu/), and in Electrical and Computer Engineering at [Shanghai Jiao Tong University](https://en.sjtu.edu.cn/). 

My research interests lie in multimodal learning and continual learning. 

News
======

* [October 2025] [MoDE](https://neurips.cc/virtual/2025/poster/119308) got accepted by [NeurIPS 2025](https://neurips.cc/). See you in San Diego! 
* [November 2024] [Online-LoRA](https://github.com/Christina200/Online-LoRA-official.git) got accepted by [WACV](https://wacv2025.thecvf.com/). See you in Tucson!
* [October 2024] Two papers got accepted by [2nd Workshop on Regulatable ML](https://regulatableml.github.io/) and [Continual FoMo Workshop](https://sites.google.com/view/continual-fomo-workshop) @NeurIPS2024. See you in Vancouver!

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

