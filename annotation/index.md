---
layout: default
title: Annotation Effort Type
---

# Dataset Directory

## Annotation Type

{% assign by_annotation = site.data.datasets | group_by: "annotation_type" %}
{% for ann in by_annotation %}
### {{ ann.name }}

{% for item in ann.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}