---
layout: 'layouts/base.njk'
title: 'Post'
---

# Post

{%- for post in posts -%}

<div class="post">
    <h2>{{ post.title }}</h2>
    <p>{{ post.body }}</p>
</div>
{%- endfor -%}
