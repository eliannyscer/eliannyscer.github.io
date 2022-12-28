---
title: "My blog"
layout: splash
permalink: /

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
 
intro: 
  - excerpt: 'Hello'
feature_row:
  - image_path: 
    alt: "placeholder image 1"
    title: "Python"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path:
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Power BI"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"

---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
