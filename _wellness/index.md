---
layout: wellness/blog
title: wellness - blog
---
{% assign posts = site.wellness 
  | where_exp: "item", "item.layout contains 'post'"  
%}
{% assign sorted_posts = posts | reverse %}

{% include wellness/blog.html post_list=sorted_posts %} 