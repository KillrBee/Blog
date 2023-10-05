---
layout: home
title: Index of HTML files
---
<main class="page-content" aria-label="Content">
     <div class="wrapper">
         # Index of HTML files
        {%- include header.html -%}
        <ul>
        {% for file in site.static_files %}
            {% if file.extname == ".html" %}
                <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.name }}</a></li>
            {% endif %}
        {% endfor %}
        </ul>
  </div>
