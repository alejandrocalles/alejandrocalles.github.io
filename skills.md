---
layout: page
title: Skills
---

{% for skill in site.data.skills %}
**{{ skill.title }}**

{{ skill.description }}
{% endfor %}
