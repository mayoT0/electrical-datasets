---
layout: default
title: Annotation Effort Type
---

# Dataset Directory

## Annotation Type

### Power - Synthetic

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Synthetic" %}
{% for ann in filtered_power_syn %}
### {{ ann_power_syn.name }}

{% for item in ann_power_syn.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}

### Power - Anonymized

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Anonymized" %}
{% for ann in filtered_power_anon %}
### {{ ann_power_anon.name }}

{% for item in ann_power_anon.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}

### Power - Compiled/Curated

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Curated" %}
{% for ann in filtered_power_curated %}
### {{ ann_power_curated.name }}

{% for item in ann_power_curated.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}

### Power - Synthetic

{% assign filtered_power_syn = site.data.datasets | where: "domain", "Power" | where: "annotation_type", "Annotated" %}
{% for ann in filtered_power_annonate %}
### {{ ann_power_annotate.name }}

{% for item in ann_power_annoate.items %}
| {{ item.title }} | [Link]({{ item.url }}) |
{% endfor %}
{% endfor %}
