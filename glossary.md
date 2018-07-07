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

{% assign something = "something" %}

{% assign allitems = "" | split:"" %}
{% for item in site.glossary %}
  {% assign allitems = allitems | push: "foo" %}
  {% assign something = "somethingelse2" %}
{% endfor %}


-->

There are {{ allitems | size }} foos ({{ something }}).
