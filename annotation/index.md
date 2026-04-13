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
{% for item in power_synthetic %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endif %}


### Power - Anonymized

{% assign power_anonymized = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Anonymized" %}

{% if power_anonymized.size > 0 %}
{% for item in power_anonymized %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endif %}

### Power - Compiled/Curated

{% assign power_compilation = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Curated" %}

{% if power_compilation.size > 0 %}
{% for item in power_compilation %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endif %}


### Power - Annotated

{% assign power_human = site.data.datasets
  | where: "domain", "Power"
  | where: "annotation_type", "Annotated" %}

{% if power_human.size > 0 %}
{% for item in power_human %}
| {{ item.title }} | {{ item.url }} |
{% endfor %}
{% endif %}

