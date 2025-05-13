---
layout: home
---

<div id="greeting" markdown="1">
# hi there, this is gabriel
</div>

<div class="home-section" id="skills" markdown="1">

# Skills

Some of the skills I've acquired over the past few years.


{% for skill in site.data.skills %}
{% assign categories = skill.categories | join: " " %}
{% if categories contains site.topic %}
<div class="skill-section" markdown="1">
## {{ skill.title }}
{{ skill.description }}
</div>
{% endif %}
{% endfor %}

</div>


<div class="home-section" id="projects" markdown="1">

# Projects

Some of the projects I've worked on.

{% for project in site.data.projects %}
[{{ project.title }}]({{ project.url | relative_url }})
{% endfor %}

</div>

