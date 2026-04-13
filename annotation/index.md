---
layout: default
title: Annotation Effort Type
---

## Annotation Type

### Power - Synthetic

{% assign power_synthetic = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Synthetic" %}

{% if power_synthetic.size > 0 %}
{% for syn in power_synthetic %}
### {{ syn.name }}
{% for item in syn.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}


### Power - Anonymized

{% assign power_anonymized = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Anonymized" %}

{% if power_anonymized.size > 0 %}
{% for item in power_anonymized %}
### {{ anon.name }}
{% for item in anon.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}

### Power - Compiled/Curated

{% assign power_compilation = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Curated" %}

{% if power_compilation.size > 0 %}
{% for item in power_compilation %}
### {{ comp.name }}
{% for item in comp.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}


### Power - Annotated

{% assign power_human = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Annotated" %}

{% if power_human.size > 0 %}
{% for item in power_human %}
### {{ human.name }}
{% for item in human.items %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endfor %}
