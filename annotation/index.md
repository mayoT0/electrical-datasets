---
layout: default
title: Annotation Effort Type
---

# Dataset Directory

## Annotation Type

### Power - Synthetic

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Synthetic" %}
{% for ann in filtered_power_syn %}
### {{ ann.name }}

{% for item in ann.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}

### Power - Anonymized

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Anonymized" %}
{% for ann1 in filtered_power_anon %}
### {{ ann1.name }}

{% for item in ann1.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}

### Power - Compiled/Curated

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Curated" %}
{% for ann2 in filtered_power_curated %}
### {{ ann2.name }}

{% for item in ann2.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}

### Power - Synthetic

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Annotated" %}
{% for ann3 in filtered_power_annonate %}
### {{ ann3.name }}

{% for item in ann3.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}
