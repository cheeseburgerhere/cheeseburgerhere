---
layout: default
title: Neural Network Dreams of Bad Apple
permalink: /bad-apple/
---

{% capture article %}{% include_relative ba_blog_assets/BLOG_POST.md %}{% endcapture %}
{% assign asset_root = '/ba_blog_assets/' | relative_url %}
{% assign video_prefix = '(' | append: asset_root | append: 'videos/' %}
{% assign figure_prefix = '(' | append: asset_root | append: 'figures/' %}
{% assign table_prefix = '(' | append: asset_root | append: 'tables/' %}
{% assign article = article | replace: '(videos/', video_prefix %}
{% assign article = article | replace: '(figures/', figure_prefix %}
{% assign article = article | replace: '(tables/', table_prefix %}

{{ article }}
