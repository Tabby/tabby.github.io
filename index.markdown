---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# TODO: group posts by month and year

layout: default
---
# Recent posts

{% for post in site.posts %}

* [{{ post.title }}]({{ post.url }})

    {{ post.description }}

    <span class="post-metadata">
    *{{ post.date | date: "%A, %B %e, %Y" }}*

{% endfor %}
