---
title: tag pages
---
# tag pages

<ul>
  {% for tag_page in site.tag_pages %}
    <li>
      <a href="{{ tag_page.url }}">
        {{ tag_page.name }}
      </a>
    </li>
  {% endfor %}
</ul>
