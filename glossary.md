---
permalink: /glossary/index.html
---

# Full list of glossary terms:

## Glossary

<ul>
{% for item in site.glossary %}
   <li><a href="{{ item.url }}">{{ item.title }}</a> — {{ item.oneliner }}</li>
{% endfor %}
</ul>

<!--

{% assign allitems = [] %}

{% for item in site.glossary %}
  {% assign allitems = allitems | concat: item %}
{% endfor %}

There are {{ allitems | size }} items.

-->
