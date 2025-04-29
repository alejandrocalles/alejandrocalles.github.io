---
layout: home
---

```bash
> whoami
gabriel
```

# Skills {#skills}

Some of the skills I've acquired over the past few years.

{% for skill in site.data.skills %}
## {{ skill.title }}

{{ skill.description }}
{% endfor %}

# Projects {#projects}

Some of the projects I've worked on.

{% for project in site.data.projects %}
[{{ project.title }}]({{ project.url | relative_url }})
{% endfor %}

