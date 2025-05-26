---
layout: home
---

<div id="greeting" markdown="1">
# hi! my name is gabriel
i'm a computer science MSc student at [EPFL](https://www.epfl.ch/en/)
specialized in data science and machine learning
</div>

<div class="home-section" id="projects" markdown="1">

# **projects**

Some of the projects I've worked on.

{% for project in site.data.projects %}
[{{ project.title }}]({{ project.url | relative_url }})
{% endfor %}

</div>

<div class="home-section" id="skills" markdown="1">

# **skills**

Some of the skills I've acquired over the past few years.


{% for skill in site.data.skills %}
{% assign categories = skill.categories | join: " " %}
{% if categories contains site.topic %}
<div class="skill-section" markdown="1">
## **{{ skill.title }}**
{{ skill.description }}
</div>
{% endif %}
{% endfor %}

</div>
