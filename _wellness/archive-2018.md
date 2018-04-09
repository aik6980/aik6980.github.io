---
layout: wellness/blog
title: wellness - archive
archive: 2018
---
{% assign groups = site.wellness
    | where_exp: "item", "item.layout contains 'post'"
    | group_by_exp:"item", "item.date | date: '%Y'"
%}

{% for group in groups %}
    {% if group.name contains page.archive %}
        {% assign posts = group.items %}
        {% break %}
    {% endif %}
{% endfor %}

{% assign sorted_posts = posts | reverse %}

{% include wellness/blog.html post_list=sorted_posts %} 