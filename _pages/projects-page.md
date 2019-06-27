---
title: "Projects"
layout: splash
permalink: /projects-page/
date: 2016-03-23T11:48:41-04:00
# header:
#  overlay_color: "#000"
#  overlay_filter: "0.5"
#  overlay_image: /assets/images/unsplash-image-1.jpg
#  actions:
#    - label: "Download"
#      url: "https://github.com/mmistakes/minimal-mistakes/"
#  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
# excerpt: "Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop."
# intro: 
#   - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
# feature_row:
#  - image_path: assets/images/unsplash-gallery-image-1-th.jpg
#    alt: "placeholder image 1"
#    title: "Placeholder 1"
#    excerpt: "This is some sample content that goes here with **Markdown** formatting."
#  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
#    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
#    alt: "placeholder image 2"
#    title: "Placeholder 2"
#    excerpt: "This is some sample content that goes here with **Markdown** formatting."
#    url: "#test-link"
#    btn_label: "Read More"
#    btn_class: "btn--primary"
#  - image_path: /assets/images/unsplash-gallery-image-3-th.jpg
#    title: "Placeholder 3"
#    excerpt: "This is some sample content that goes here with **Markdown** formatting."
projects:
    row_1:
        - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
          alt: "placeholder image 2"
          title: "Transcription elongation factor Spt6"
          excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
          url: "#test-link"
          btn_label: "Read More"
          btn_class: "btn--primary"
    row_2:
        - #image_path: /assets/images/unsplash-gallery-image-2-th.jpg
          #alt: "placeholder image 2"
          title: "Transcription elongation factor Spt5"
          excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
          url: "#test-link"
          btn_label: "Read More"
          btn_class: "btn--primary"
    row_3:
        - # image_path: /assets/images/unsplash-gallery-image-2-th.jpg
          # alt: "placeholder image 3"
          title: "Functions of intragenic transcription"
          excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
          url: "#test-link"
          btn_label: "Read More"
          btn_class: "btn--primary"
    row_4:
        - # image_path: /assets/images/unsplash-gallery-image-2-th.jpg
          # alt: "placeholder image 3"
          title: "DNA assembly methods"
          excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
          url: "#test-link"
          btn_label: "Read More"
          btn_class: "btn--primary"
---

Projects that I've worked on or am currently working on.

{% for p in page.projects %}
    {% assign project=p[0] %}
    {% include feature_row id=project type="right" %}
{% endfor %}

