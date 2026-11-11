---
title: tags
layout: page
---
# tags

test tags description

<ul>
  {% assign sorted_tags = site.tags | sort %}

  {% for tag in sorted_tags %}
    {% assign tag_name = tag[0] %}
    {% assign tag_page = site.tag_pages | where: "title", tag_name | first %}

    {% if tag_page %}
      <li>
        <a href="{{ tag_page.url }}">{{ tag_name }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>