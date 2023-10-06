---
layout: home
title: Published Works
---
<main class="page-content" aria-label="Content">
     <div class="wrapper">
         These are some of my published works on Medium.com
        {%- include header.html -%}
        <ul>
        {% for file in site.static_files %}
            {% if file.extname == ".html" %}
                <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
            {% endif %}
        {% endfor %}
        </ul>
  </div>
