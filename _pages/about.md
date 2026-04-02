---
permalink: /
title: ""
excerpt: "M.S. Student @ HIT | 3D Vision & VLM Research"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div id="about"></div>

About me
======

Welcome! I am Jiaxin Zhang(张佳鑫), a master student in Computer Science at [Harbin Institute of Technology (HIT)](https://www.hit.edu.cn/), supervised by [Prof. Junjun Jiang](https://homepage.hit.edu.cn/jiangjunjun). Currently, I am an intern at the Multimodal Large Model Lab of Huawei 2012 Laboratories, where I am mentored by [Dave Zhenyu Chen](https://daveredrum.github.io/). Prior to this, I earned my Bachelor’s degree in Computer Science from [HIT](https://www.hit.edu.cn/).

My research interests focus on **3D reconstruction** and **vision-language model (VLM)-based 3D spatial perception and reasoning**. Beyond research, I am a backpacker—either my body or my mind is always on the road.

<div id="internships"></div>

Internships
======

* 2025.05 - 2026.04: Research Intern
  * Huawei 2012 Laboratories, Huawei
  * Department: Multimodal Large Model Lab
  * Supervisor: [Dave Zhenyu Chen](https://daveredrum.github.io/)
  
<div id="awards"></div>

Selected Award
======

* China **National** Scholarship, 2025
* **Special-Class** Scholarship for Postgraduate Students, 2024, 2025(**Top 0.3%**)
* **Outstanding Graduate** of Heilongjiang Province, China, 2024
* The **First-class** Scholarship at Harbin Institute of Technology, 2022, 2023
* **Tencent** Scholarship, 2023
  
<div id="publications"></div>

Publications
======


{% assign pubs = site.publications | sort: "date" | reverse %}

{% for post in pubs %}
<table style="border: 0; border-collapse: collapse; margin-bottom: 1.5em;">
  <tr style="border: 0;">
    <td width="30%" style="border: 0; padding-right: 20px; vertical-align: top;">
      {% if post.header.teaser %}
      <img src="/images/{{ post.header.teaser }}" width="100%" style="max-width: 220px; border-radius: 6px;">
      {% endif %}
    </td>
    <td width="70%" style="border: 0; vertical-align: top;">
      <strong>{{ post.title }}</strong><br>
      
      {% if post.authors %}
      {{ post.authors }}<br>
      {% endif %}
      
      {% if post.venue %}
      <em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}<br>
      {% endif %}
      
      {% if post.excerpt %}
      <div style="margin-top: 0.4em; margin-bottom: 0.4em;">
        {{ post.excerpt }}
      </div>
      {% endif %}
      
      {% if post.paperurl %}
      <a href="{{ post.paperurl }}">[Paper]</a>
      {% endif %}
      
      {% if post.codeurl %}
      <a href="{{ post.codeurl }}">[Code]</a>
      {% endif %}
      
      {% if post.projecturl %}
      <a href="{{ post.projecturl }}">[Project]</a>
      {% endif %}
      
      {% if post.slidesurl %}
      <a href="{{ post.slidesurl }}">[Slides]</a>
      {% endif %}
    </td>
  </tr>
</table>
{% endfor %}