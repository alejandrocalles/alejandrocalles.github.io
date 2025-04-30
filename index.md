---
layout: home
---

<div></div>

# Skills {#skills}

Some of the skills I've acquired over the past few years.


{% for skill in site.data.skills %}
{% assign categories = skill.categories | join: " " %}
{% if categories contains site.topic %}
## {{ skill.title }}
{{ skill.description }}
{% endif %}
{% endfor %}

# Projects {#projects}

Some of the projects I've worked on.

{% for project in site.data.projects %}
[{{ project.title }}]({{ project.url | relative_url }})
{% endfor %}

