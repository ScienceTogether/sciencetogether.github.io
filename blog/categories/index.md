---
layout: default
---

<h1>Categories</h1>

{% for category in site.categories %}[{{ category | first}}](/blog/categories/#{{category | first | slugize}})  {% endfor %}


{% for category in site.categories %}
{% assign categ = category | first | slugize %}

### {{ categ }}

 {% for post in site.categories[categ] %}
 - {{ post.date | date_to_string }}: [{{post.title}}]({{ post.url}})
 {% endfor %}
{% endfor %}
