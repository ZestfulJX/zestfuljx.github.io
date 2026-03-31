---
permalink: /
title: "Jiaxin Zhang"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<section id="About Me" style="scroll-margin-top: 80px;">
## About Me

I am Jiaxin Zhang, a Master's student in Computer Science and Technology at Harbin Institute of Technology, where I am advised by Prof. Junjun Jiang. I am currently interning at Huawei, under the supervision of Dave Zhenyu Chen. My research interests include 3D reconstruction and understanding, multimodal large models, geometric alignment, and 3D scene representation.

I received my B.E. in Computer Science and Technology, Intelligent Information Processing, from Harbin Institute of Technology in `2024`, with a GPA of `3.89 / 4.00`.

I am currently looking for `27 Fall PhD` opportunities.
</section>

<section id="Internships" style="scroll-margin-top: 80px;">
## Internships

- **Huawei 2012 Laboratories, Multimodal Model Lab**  
  `2025.05 - 2026.03`

  Worked on integrating feed-forward 3D reconstruction with vision-language models to improve 3D spatial perception and spatial understanding. This work contributed to the paper *GAP-MLLM*.
</section>

<section id="Honors and Awards" style="scroll-margin-top: 80px;">
## Honors and Awards

- National Scholarship, `2025.12`
- Heilongjiang Provincial Merit Student, `2025.11`
- HIT Graduate Special Scholarship `(1/330)`, `2025.09`
- Huawei Intelligent Base Scholarship, `2024.09`
- Tencent Scholarship, `2023.01`
</section>

<section id="publications" style="scroll-margin-top: 80px;">
## Publications

{% if site.author.googlescholar %}
You can also find my articles on [Google Scholar]({{ site.author.googlescholar }}).
{% endif %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
### {{ category[1].title }}
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
</section>
