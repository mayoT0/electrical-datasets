---
layout: default
title: Data Format & Structure
---

# Dataset Directory

## Format

{% assign by_format = site.data.datasets | group_by: "data_format" %}
{% for format in by_format %}
### {{ format.name }}

{% for item in format.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}