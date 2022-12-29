---
title: "My blog"
layout: splash
permalink: /

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/mean_stack.png
  excerpt: "Articles and tutorials about python and data analysis"
 
intro: 
  - excerpt: ""
feature_row:
  - image_path: /assets/images/python.jpg
    alt: "placeholder image 1"
    title: "Python"
    excerpt: "It is a very popular programming language because it is incredibly productive and efficient."
    url: "/tags/#python"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/power-bi.png
    alt: "placeholder image 2"
    title: "Power BI"
    excerpt: "It provides interactive visualizations and high-end analytics capabilities that help everyone to make smarter, real-time decisions."
    url: ""
    btn_label: "Comming soon.."
    btn_class: "btn--primary"


---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
