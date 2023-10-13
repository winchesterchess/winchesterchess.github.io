---
title: "" # Prevents "News" from being the page title
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/exhibition.jpeg
  actions:
    - label: "Join us"
      url: "/join/"
#   caption: "Photo credit: [**Somebody**](https://example.com)"
excerpt: >
    Has the recent chess boom rekindled your interest? Why not try some friendly
    games, or take the next step and set your over the board rating!
---
## News

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

{% include paginator.html %}
