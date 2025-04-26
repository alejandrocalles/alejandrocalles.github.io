---
layout: page
title: Skills
description: "Some of the skills I've acquired over the past few years."
---

{% for skill in site.data.skills %}
**{{ skill.title }}**

{{ skill.description }}
{% endfor %}
