---
layout: 'layouts/base.njk'
title: 'Home'
---

# Home

<ul>
    {%- for page in collections.static -%}
    <!-- tags: static privacy  -->
        <!-- <li>
            <a href="{{ page.url }}">
                {{ page.data.title }}
            </a>
        </li> -->
    {%- endfor -%}
</ul>

{% for post in collections.posts %} - [{{ post.data.title }}]({{ post.url }}){% endfor %}

<footer>Copyright {{ site.year }}, all rights reserved.</footer>
