---
layout: page
permalink: wiki/
---

{% assign pages_with_category = site.about | where_exp: "item", "item.category" %}
{% assign categories = pages_with_category | map: "category" | uniq %}
{% for category in categories %}
## {{ category }}
{% assign sorted_pages = pages_with_category | where: "category", category | sort: "title" %}
{% for page in sorted_pages %}
* <a href="{{ page.url | relative_url }}"> [{{ page.title }}]({{ page.url | relative_url }})</a>
{% endfor %}
{% endfor %}