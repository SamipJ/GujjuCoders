---
layout: default
---

## Articles[.]({{ site.baseurl }}/archive)
{% assign posts = 0 %} {% for post in site.posts %} {% if post.category == "Blog"%}

* [{{ post.title }}]({{ site.baseurl}}{{ post.url }}) {% assign posts = posts | plus: 1 %} {% endif %} {% if posts == 5 %} {% break %} {% endif %}
{% endfor %}

## Notes 
{% assign posts = 0 %} {% for post in site.posts %} {% if post.category == "Notes"%}

* [{{ post.title }}]({{ site.baseurl}}{{ post.url }}) {% assign posts = posts | plus: 1 %} {% endif %} {% if posts == 3 %} {% break %} {% endif %}
{% endfor %}


