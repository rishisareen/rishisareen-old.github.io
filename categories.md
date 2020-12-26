---
layout: page
permalink: /categories/
title: Categories
sidebar_link: true
---


<div id="archives">
{% for category in site.categories %}
    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
  		* {{ post.date | date_to_string }} &mdash; [ {{ post.title }} ]({{ post.url }})
    {% endfor %}
{% endfor %}
</div>
