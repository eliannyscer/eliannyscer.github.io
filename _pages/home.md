---
title: "My blog"
layout: splash
permalink: /

header:
  overlay_color: "#5e616c"
  overlay_filter: "0.5"
  overlay_image: /assets/images/bio-photo.jpg
 
intro: 
  - excerpt: ''
feature_row:
  - image_path: /assets/images/python.jpg
    alt: "placeholder image 1"
    title: "Python"
    excerpt: ""
    url: "/tags/#python"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/power-bi.png
    alt: "placeholder image 2"
    title: "Power BI"
    excerpt: ""
    url: ""
    btn_label: "Comming soon.."
    btn_class: "btn--primary"


---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
