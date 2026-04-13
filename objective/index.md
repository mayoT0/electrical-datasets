---
layout: default
title: Dataset Objective
---

# Dataset Objective

## Objective

{% assign by_objective = site.data.datasets | group_by: "objective" %}
{% for obj in by_objective %}
### {{ obj.name }}

{% for item in obj.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}
