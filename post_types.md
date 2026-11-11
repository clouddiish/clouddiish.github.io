---
title: post types
layout: base
---
# post types

test post types description

<ul>
  {% assign sorted_post_type_pages = site.post_type_pages | sort %}

  {% for post_type_page in sorted_post_type_pages %}
    {% assign post_type_name = post_type_page.title %}
    <li>
      <a href="{{ post_type_page.url }}">{{ post_type_name }}</a>
    </li>
  {% endfor %}
</ul>