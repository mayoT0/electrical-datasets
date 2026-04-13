
---
layout: default
title: Dataset Objective
---

{{ '/assets/images/objective.jpg' | relative_url }}

# Dataset Directory

## Objective

{% assign by_objective = site.data.datasets | group_by: "objective" %}
{% for obj in by_objective %}
### {{ obj.name }}

{% for item in obj.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}